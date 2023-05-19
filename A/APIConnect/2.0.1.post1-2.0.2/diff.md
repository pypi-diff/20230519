# Comparing `tmp/APIConnect-2.0.1.post1.tar.gz` & `tmp/APIConnect-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\APIConnect-2.0.1.post1.tar", last modified: Mon Feb  6 10:50:12 2023, max compression
+gzip compressed data, was "APIConnect-2.0.2.tar", last modified: Fri May 19 16:53:15 2023, max compression
```

## Comparing `APIConnect-2.0.1.post1.tar` & `APIConnect-2.0.2.tar`

### file list

```diff
@@ -1,55 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-02-06 10:50:12.000000 APIConnect-2.0.1.post1/
-drwxrwxrwx   0        0        0        0 2023-02-06 10:50:12.000000 APIConnect-2.0.1.post1/APIConnect/
--rw-rw-rw-   0        0        0    73252 2023-02-06 10:45:21.000000 APIConnect-2.0.1.post1/APIConnect/APIConnect.py
--rw-rw-rw-   0        0        0     1727 2022-12-16 20:42:27.000000 APIConnect-2.0.1.post1/APIConnect/api_utils.py
--rw-rw-rw-   0        0        0     6645 2022-12-16 20:42:27.000000 APIConnect-2.0.1.post1/APIConnect/http.py
--rw-rw-rw-   0        0        0     5276 2022-12-16 20:42:27.000000 APIConnect-2.0.1.post1/APIConnect/login_helper.py
--rw-rw-rw-   0        0        0     3952 2022-12-16 20:42:27.000000 APIConnect-2.0.1.post1/APIConnect/order.py
--rw-rw-rw-   0        0        0     4417 2022-12-16 20:42:27.000000 APIConnect-2.0.1.post1/APIConnect/validator.py
-drwxrwxrwx   0        0        0        0 2023-02-06 10:50:12.000000 APIConnect-2.0.1.post1/APIConnect.egg-info/
--rw-rw-rw-   0        0        0      897 2023-02-06 10:50:12.000000 APIConnect-2.0.1.post1/APIConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1129 2023-02-06 10:50:12.000000 APIConnect-2.0.1.post1/APIConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-06 10:50:12.000000 APIConnect-2.0.1.post1/APIConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-02-06 10:50:12.000000 APIConnect-2.0.1.post1/APIConnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       56 2023-02-06 10:50:12.000000 APIConnect-2.0.1.post1/APIConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1156 2023-02-03 06:14:11.000000 APIConnect-2.0.1.post1/LICENSE.txt
--rw-rw-rw-   0        0        0      897 2023-02-06 10:50:12.000000 APIConnect-2.0.1.post1/PKG-INFO
--rw-rw-rw-   0        0        0       41 2022-07-27 12:36:50.000000 APIConnect-2.0.1.post1/README
-drwxrwxrwx   0        0        0        0 2023-02-06 10:50:12.000000 APIConnect-2.0.1.post1/conf/
--rw-rw-rw-   0        0        0      365 2023-02-06 10:36:45.000000 APIConnect-2.0.1.post1/conf/settings.ini
-drwxrwxrwx   0        0        0        0 2023-02-06 10:50:12.000000 APIConnect-2.0.1.post1/constants/
--rw-rw-rw-   0        0        0      181 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/constants/action.py
--rw-rw-rw-   0        0        0      380 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/constants/asset_type.py
--rw-rw-rw-   0        0        0      292 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/constants/chart_exchange.py
--rw-rw-rw-   0        0        0      638 2023-02-03 11:49:59.000000 APIConnect-2.0.1.post1/constants/constants.py
--rw-rw-rw-   0        0        0      234 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/constants/duration.py
--rw-rw-rw-   0        0        0      203 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/constants/eod_Interval.py
--rw-rw-rw-   0        0        0      255 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/constants/exchange.py
--rw-rw-rw-   0        0        0      260 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/constants/intraday_interval.py
--rw-rw-rw-   0        0        0      237 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/constants/market_cap.py
--rw-rw-rw-   0        0        0      255 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/constants/order_type.py
--rw-rw-rw-   0        0        0      251 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/constants/product_code.py
--rw-rw-rw-   0        0        0      244 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/constants/results_stocks_news_category.py
--rw-rw-rw-   0        0        0     9121 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/constants/router.py
--rw-rw-rw-   0        0        0      215 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/constants/segment.py
--rw-rw-rw-   0        0        0      234 2022-12-16 20:42:27.000000 APIConnect-2.0.1.post1/constants/streaming_constants.py
--rw-rw-rw-   0        0        0      242 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/constants/term.py
-drwxrwxrwx   0        0        0        0 2023-02-06 10:50:12.000000 APIConnect-2.0.1.post1/exceptions/
--rw-rw-rw-   0        0        0      185 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/exceptions/api_exception.py
--rw-rw-rw-   0        0        0      397 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/exceptions/validation_exception.py
-drwxrwxrwx   0        0        0        0 2023-02-06 10:50:12.000000 APIConnect-2.0.1.post1/feed/
--rw-rw-rw-   0        0        0     6113 2023-02-06 10:45:28.000000 APIConnect-2.0.1.post1/feed/feed.py
--rw-rw-rw-   0        0        0     1624 2022-12-16 20:42:27.000000 APIConnect-2.0.1.post1/feed/livenews_feed.py
--rw-rw-rw-   0        0        0     2105 2022-12-16 20:42:27.000000 APIConnect-2.0.1.post1/feed/orders_feed.py
--rw-rw-rw-   0        0        0     2151 2022-12-16 20:42:27.000000 APIConnect-2.0.1.post1/feed/quotes_feed.py
-drwxrwxrwx   0        0        0        0 2023-02-06 10:50:12.000000 APIConnect-2.0.1.post1/resources/
--rw-rw-rw-   0        0        0     1146 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/resources/chart_response_formatter.py
--rw-rw-rw-   0        0        0     4748 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/resources/live_news_resource.py
--rw-rw-rw-   0        0        0     1537 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/resources/research_calls_resource.py
--rw-rw-rw-   0        0        0      926 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/resources/watchlist_resource.py
-drwxrwxrwx   0        0        0        0 2023-02-06 10:50:12.000000 APIConnect-2.0.1.post1/services/
--rw-rw-rw-   0        0        0     9531 2022-12-16 20:42:27.000000 APIConnect-2.0.1.post1/services/live_news_service.py
--rw-rw-rw-   0        0        0     2425 2022-10-07 08:39:52.000000 APIConnect-2.0.1.post1/services/research_calls_service.py
--rw-rw-rw-   0        0        0     9751 2022-12-16 20:42:27.000000 APIConnect-2.0.1.post1/services/watchlist_service.py
--rw-rw-rw-   0        0        0       42 2023-02-06 10:50:12.000000 APIConnect-2.0.1.post1/setup.cfg
--rw-rw-rw-   0        0        0     1213 2023-02-06 10:48:33.000000 APIConnect-2.0.1.post1/setup.py
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.320442 APIConnect-2.0.2/
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.285652 APIConnect-2.0.2/APIConnect/
+-rw-r--r--   0 saurabh    (502) staff       (20)    66126 2023-05-19 14:30:01.000000 APIConnect-2.0.2/APIConnect/APIConnect.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     1877 2023-05-03 11:18:05.000000 APIConnect-2.0.2/APIConnect/api_constants.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     3234 2023-05-03 11:18:05.000000 APIConnect-2.0.2/APIConnect/api_utils.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     6501 2023-03-16 11:10:11.000000 APIConnect-2.0.2/APIConnect/http.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     5379 2023-05-03 11:18:05.000000 APIConnect-2.0.2/APIConnect/login_helper.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     3788 2023-03-23 11:20:24.000000 APIConnect-2.0.2/APIConnect/order.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     4696 2023-05-03 11:18:05.000000 APIConnect-2.0.2/APIConnect/validator.py
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.289817 APIConnect-2.0.2/APIConnect.egg-info/
+-rw-r--r--   0 saurabh    (502) staff       (20)      833 2023-05-19 16:53:15.000000 APIConnect-2.0.2/APIConnect.egg-info/PKG-INFO
+-rw-r--r--   0 saurabh    (502) staff       (20)     1022 2023-05-19 16:53:15.000000 APIConnect-2.0.2/APIConnect.egg-info/SOURCES.txt
+-rw-r--r--   0 saurabh    (502) staff       (20)        1 2023-05-19 16:53:15.000000 APIConnect-2.0.2/APIConnect.egg-info/dependency_links.txt
+-rw-r--r--   0 saurabh    (502) staff       (20)       33 2023-05-19 16:53:15.000000 APIConnect-2.0.2/APIConnect.egg-info/requires.txt
+-rw-r--r--   0 saurabh    (502) staff       (20)       56 2023-05-19 16:53:15.000000 APIConnect-2.0.2/APIConnect.egg-info/top_level.txt
+-rw-r--r--   0 saurabh    (502) staff       (20)     1140 2023-03-16 11:10:11.000000 APIConnect-2.0.2/LICENSE.txt
+-rw-r--r--   0 saurabh    (502) staff       (20)      833 2023-05-19 16:53:15.319292 APIConnect-2.0.2/PKG-INFO
+-rw-r--r--   0 saurabh    (502) staff       (20)       40 2023-03-16 11:10:11.000000 APIConnect-2.0.2/README
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.290363 APIConnect-2.0.2/conf/
+-rw-r--r--   0 saurabh    (502) staff       (20)      354 2023-05-19 10:57:43.000000 APIConnect-2.0.2/conf/settings.ini
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.304233 APIConnect-2.0.2/constants/
+-rw-r--r--   0 saurabh    (502) staff       (20)      173 2023-05-03 11:18:05.000000 APIConnect-2.0.2/constants/action.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      363 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/asset_type.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      278 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/chart_exchange.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      624 2023-05-19 10:58:48.000000 APIConnect-2.0.2/constants/constants.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      222 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/duration.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      193 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/eod_Interval.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      242 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/exchange.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      247 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/intraday_interval.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      244 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/order_type.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      238 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/product_code.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      236 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/results_stocks_news_category.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     8275 2023-05-03 11:18:05.000000 APIConnect-2.0.2/constants/router.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      224 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/streaming_constants.py
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.306627 APIConnect-2.0.2/exceptions/
+-rw-r--r--   0 saurabh    (502) staff       (20)      180 2023-03-16 11:10:11.000000 APIConnect-2.0.2/exceptions/api_exception.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      384 2023-03-16 11:10:11.000000 APIConnect-2.0.2/exceptions/validation_exception.py
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.312050 APIConnect-2.0.2/feed/
+-rw-r--r--   0 saurabh    (502) staff       (20)     5961 2023-05-19 14:29:36.000000 APIConnect-2.0.2/feed/feed.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     1577 2023-03-16 11:10:11.000000 APIConnect-2.0.2/feed/livenews_feed.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     2046 2023-03-16 11:10:11.000000 APIConnect-2.0.2/feed/orders_feed.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     2091 2023-03-16 11:10:11.000000 APIConnect-2.0.2/feed/quotes_feed.py
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.315244 APIConnect-2.0.2/resources/
+-rw-r--r--   0 saurabh    (502) staff       (20)     1123 2023-03-16 11:10:11.000000 APIConnect-2.0.2/resources/chart_response_formatter.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     4635 2023-03-16 11:10:11.000000 APIConnect-2.0.2/resources/live_news_resource.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      901 2023-03-16 11:10:11.000000 APIConnect-2.0.2/resources/watchlist_resource.py
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.317730 APIConnect-2.0.2/services/
+-rw-r--r--   0 saurabh    (502) staff       (20)     9382 2023-05-03 11:18:05.000000 APIConnect-2.0.2/services/live_news_service.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     9505 2023-05-03 11:18:05.000000 APIConnect-2.0.2/services/watchlist_service.py
+-rw-r--r--   0 saurabh    (502) staff       (20)       38 2023-05-19 16:53:15.320667 APIConnect-2.0.2/setup.cfg
+-rw-r--r--   0 saurabh    (502) staff       (20)     1173 2023-05-19 10:55:02.000000 APIConnect-2.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `APIConnect-2.0.1.post1/APIConnect/APIConnect.py` & `APIConnect-2.0.2/APIConnect/APIConnect.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1595 +1,1471 @@
-import json
-import os
-import errno
-import sys
-from os import path
-import logging
-import configparser
-from APIConnect.http import Http, init_proxies
-from APIConnect.login_helper import LoginHelper
-from feed.feed import Feed
-from feed.quotes_feed import QuotesFeed
-from feed.orders_feed import OrdersFeed
-from feed.livenews_feed import LiveNewsFeed
-from constants.asset_type import AssetTypeEnum
-from constants.chart_exchange import ChartExchangeEnum
-from constants.market_cap import MarketCapEnum
-from constants.segment import SegmentEnum
-from constants.term import TermEnum
-from constants.router import Router
-from constants.intraday_interval import IntradayIntervalEnum
-from APIConnect.api_utils import ApiUtils
-from constants.eod_Interval import EODIntervalEnum
-from constants.exchange import ExchangeEnum
-from constants.order_type import OrderTypeEnum
-from constants.product_code import ProductCodeENum
-from constants.duration import DurationEnum
-from constants.action import ActionEnum
-from APIConnect.order import Order
-from APIConnect.validator import Validator
-from exceptions.validation_exception import ValidationException
-from resources.chart_response_formatter import ChartResponseFormatter
-from services.live_news_service import LiveNewsService
-from services.watchlist_service import WatchlistService
-from services.research_calls_service import ResearchCallsService
-
-logging.basicConfig(filename = 'apiconnect.log',
-        level=logging.DEBUG,
-        format="%(asctime)s [%(levelname)s] %(name)s: %(message)s")
-LOGGER = logging.getLogger(__name__)
-
-LOG_LEVELS = {
-    'INFO': logging.INFO,
-    'DEBUG': logging.DEBUG,
-    'ERROR': logging.ERROR,
-    'CRITICAL': logging.CRITICAL
-}
-
-def init_logger(conf) -> None:
-    """
-    Method to initialize logger configuration via provided configuration object.
-    - Parameters:\n
-    `conf`: ConfigParser object of provided settings.ini file.
-    """
-
-    LOG_LEVEL=None
-    LOG_FILE=None
-    if 'LOG_LEVEL' in conf['GLOBAL'] and conf['GLOBAL']['LOG_LEVEL'] in LOG_LEVELS:
-        LOG_LEVEL = LOG_LEVELS[conf['GLOBAL']['LOG_LEVEL']]
-    if 'LOG_FILE' in conf['GLOBAL']:
-        LOG_FILE = conf['GLOBAL']['LOG_FILE']
-    if LOG_FILE or LOG_LEVEL:
-        for handler in logging.root.handlers[:]:
-            logging.root.removeHandler(handler)
-        LOG_FILE = LOG_FILE if LOG_FILE else 'apiconnect.log'
-        LOG_LEVEL = LOG_LEVEL if LOG_LEVEL else logging.INFO
-        logging.basicConfig(filename=LOG_FILE, level=LOG_LEVEL,
-                format="%(asctime)s [%(levelname)s] %(name)s: %(message)s")
-
-class APIConnect:
-
-    def __init__(self, ApiKey, Password, reqID, downloadContract: bool, conf = None) -> None:
-        self.__conf = None
-        self.__init_logger = init_logger
-        if conf:
-            self.__conf = configparser.ConfigParser()
-            try:
-                if path.exists(conf):
-                    self.__conf.read(conf)
-                    self.__init_logger(self.__conf)
-                    LOGGER.info("Loggers initiated with provided configuration.")
-                else:
-                    raise FileNotFoundError(
-                        errno.ENOENT, os.strerror(errno.ENOENT), conf)
-            except Exception as ex:
-                LOGGER.exception("Error occurred while parsing provided configuaration file: %s", ex)
-                raise ex
-        else:
-            LOGGER.info("Logger initiated with default values.")
-
-        self.__version = '2.0.1'
-        self.__dc = downloadContract
-        self.__filename = "data_" + ApiKey + '.txt'
-        self.__router = Router(self.__conf)
-        self.__constants = ApiUtils()
-        self.__init_proxies = init_proxies
-        self.__proxies = self.__init_proxies(self.__conf)
-        self.__http = Http(self.__constants, self.__proxies)
-        self.__constants.Filename = self.__filename
-        self.__constants.ApiKey = ApiKey
-        self.__login_helper = LoginHelper(self.__http, self.__router, self.__constants)
-        AppIdKey = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhcHAiOjAsImZmIjoiVyIsImJkIjoid2ViLXBjIiwibmJmIjoxNjcxMTcwMjc2LCJzcmMiOiJlbXRtdyIsImF2IjoiMi4wLjAiLCJhcHBpZCI6IjQxZGE0MDEyNDg2YjFhY2IzNTc4YzYwZjdmNGUyNDhhIiwiaXNzIjoiZW10IiwiZXhwIjoxNjcxMjE1NDAwLCJpYXQiOjE2NzExNzA1NzZ9.7mqgyIfCxuILFGKI_WR0QsrS64mUIKptW5D7utHyDHA"
-
-        if conf and self.__conf['GLOBAL'].get('AppIdKey'):
-            AppIdKey = self.__conf['GLOBAL'].get('AppIdKey')
-        self.__constants.AppIdKey = AppIdKey
-
-        if path.exists(self.__filename):
-            LOGGER.info("User data file found, loading data.")
-            read = open(self.__filename, 'r').read()
-            j = json.loads(read)
-            self.__constants.VendorSession = j['vt']
-            self.__constants.JSessionId =  j['auth']
-            self.__constants.eqAccId = j['eqaccid']
-            self.__constants.coAccId = j['coaccid']
-            self.__constants.Data = j['data']
-            self.__constants.ProfileId = j.get('data').get('data').get('lgnData').get('accs').get('prfId')
-            self.__constants.AppIdKey = j['appidkey']
-        else:
-            self.__login_helper._GenerateVendorSession(ApiKey, Password)
-            self.__login_helper._GetAuthorization(reqID)
-
-        self.__feedObj = Feed(self.__conf)
-
-        self.__CheckUpdate()
-
-        self.__login_helper._Instruments(self.__dc, self.__proxies)
-
-    def __CheckUpdate(self):
-        LOGGER.info("Checking for new update.")
-        url = self.__router._CheckUpdateURl()
-        rep = self.__http._PostMethod(url, json.dumps({"lib": "EAC_PYTHON", "vsn": self.__version}))
-        if rep['data']['sts'] is True:
-            if rep['data']['msg'] == 'MANDATORY':
-                print("Mandatory Update. New version " + rep['data']['vsn'] + '. Update to new version to continue.')
-                LOGGER.info("New mandatory update found. Please update to new version.")
-                sys.exit(0)
-            if rep['data']['msg'] == 'OPTIONAL':
-                LOGGER.info("New optional update found.")
-                print("New version " + rep['data']['vsn'] + " is available. Stay up to date for better experience")
-
-
-    def GetLoginData(self) -> str:
-        """
-
-        Get Login Info.
-
-        """
-        return json.dumps(self.__constants.Data)
-
-# Trade Methods
-
-    def OrderBook(self) -> str:
-        """
-
-        This method will retrieve the equity Order Book. Typical order book response will be a nested JSON containing below fields
-            - Symbol
-            - Product Type
-            - Order type
-            - Quantity
-            - Price
-            - Validity
-            - Order ID
-            - Order Status
-
-        """
-        LOGGER.info("OrderBook method is called.")
-        if self.__constants.Data['data']['lgnData']['accTyp'] == 'EQ':
-            url = self.__router._OrderBookURL().format(userid=self.__constants.eqAccId)
-            LOGGER.debug("OrderBook method is called for 'EQ' account type")
-            eq = self.__http._GetMethod(url)
-            LOGGER.debug("Response received: %s", eq)
-            return json.dumps({"eq": eq, "comm": ""})
-
-        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'CO':
-            url = self.__router._OrderBookURL_comm().format(userid=self.__constants.coAccId, reqtype='COMFNO')
-            LOGGER.debug("OrderBook method is called for 'CO' account type")
-            comm = self.__http._GetMethod(url)
-            LOGGER.debug("Response received: %s", comm)
-            return json.dumps({"eq": "", "comm": comm})
-
-        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'COMEQ':
-            url = self.__router._OrderBookURL().format(userid=self.__constants.eqAccId)
-            LOGGER.debug("OrderBook method is called for 'COMEQ' account type")
-            url_comm = self.__router._OrderBookURL_comm().format(userid=self.__constants.coAccId, reqtype='COMFNO')
-            rep = self.__http._GetMethod(url)
-            LOGGER.debug("Response for eq: %s", rep)
-            rep_comm = self.__http._GetMethod(url_comm)
-            LOGGER.debug("Response for comm: %s", rep_comm)
-            combine = {"eq": rep, "comm": rep_comm}
-            return json.dumps(combine)
-
-
-    def TradeBook(self) -> str:
-
-        """
-
-          This method will retrieve the Trade Book. Typical trade book response will be a nested JSON containing below fields
-            - Symbol
-            - Product Type
-            - Order type
-            - Quantity
-            - Price
-            - Validity
-            - Trade ID
-            - Trade Status
-
-        """
-        LOGGER.info("TradeBook method is called.")
-        if self.__constants.Data['data']['lgnData']['accTyp'] == 'EQ':
-            url = self.__router._TradeBookURL().format(userid=self.__constants.eqAccId)
-            # return json.dumps({"eq": self.__http.GetMethod(url), "comm": ""})
-            LOGGER.debug("TradeBook method is called for 'EQ' account type")
-            eq = self.__http._GetMethod(url)
-            LOGGER.debug("Response received: %s", eq)
-            return json.dumps({"eq": eq, "comm": ""})
-
-        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'CO':
-            url = self.__router._TradeBookURL_comm().format(userid=self.__constants.coAccId)
-            # return json.dumps({"eq": "", "comm": self.__http.GetMethod(url)})
-            LOGGER.debug("TradeBook method is called for 'CO' account type")
-            comm = self.__http._GetMethod(url)
-            LOGGER.debug("Response received: %s", comm)
-            return json.dumps({"eq": "", "comm": comm})
-
-        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'COMEQ':
-            url = self.__router._TradeBookURL().format(userid=self.__constants.eqAccId)
-            url_comm = self.__router._TradeBookURL_comm().format(userid=self.__constants.coAccId)
-            LOGGER.debug("TradeBook method is called for 'COMEQ' account type")
-            rep = self.__http._GetMethod(url)
-            LOGGER.debug("Response for eq: %s", rep)
-            rep_comm = self.__http._GetMethod(url_comm)
-            LOGGER.debug("Response for comm: %s", rep_comm)
-            combine = {"eq": rep, "comm": rep_comm}
-            return json.dumps(combine)
-
-
-    def NetPosition(self) -> str:
-        """
-        Net position usually is referred to in context of trades placed during the day in case of Equity, or can refer to carry forward positions in case of Derivatives, Currency and Commodity. It indicates the net obligation (either buy or sell) for the given day in a given symbol. Usually you monitor the net positions screen to track the profit or loss made from the given trades and will have options to square off your entire position and book the entire profit and loss.
-
-
-       This method will retrieve the Net position. Typical trade book response will be a nested JSON containing below fields
-            - Symbol
-            - Product Type
-            - Order type
-            - Quantity
-            - Price
-            - Validity
-            - Trade ID
-            - Trade Status
-
-          """
-        LOGGER.info("NetPosition method is called.")
-        if self.__constants.Data['data']['lgnData']['accTyp'] == 'EQ':
-            url = self.__router._NetPositionURL().format(userid=self.__constants.eqAccId)
-            # return json.dumps({"eq": self.__http.GetMethod(url), "comm": ""})
-            LOGGER.debug("NetPosition method is called for 'EQ' account type")
-            eq = self.__http._GetMethod(url)
-            LOGGER.debug("Response received: %s", eq)
-            return json.dumps({"eq": eq, "comm": ""})
-
-        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'CO':
-            url = self.__router._NetPositionURL_comm().format(userid=self.__constants.coAccId)
-            # return json.dumps({"eq": "", "comm": self.__http.GetMethod(url)})
-            LOGGER.debug("NetPosition method is called for 'CO' account type")
-            comm = self.__http._GetMethod(url)
-            LOGGER.debug("Response received: %s", comm)
-            return json.dumps({"eq": "", "comm": comm})
-
-        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'COMEQ':
-            url = self.__router._NetPositionURL().format(userid=self.__constants.eqAccId)
-            url_comm = self.__router._NetPositionURL_comm().format(userid=self.__constants.coAccId)
-            LOGGER.debug("TradeBook method is called for 'COMEQ' account type")
-            rep = self.__http._GetMethod(url)
-            LOGGER.debug("Response for eq: %s", rep)
-            rep_comm = self.__http._GetMethod(url_comm)
-            LOGGER.debug("Response for comm: %s", rep_comm)
-            combine = {"eq": rep, "comm": rep_comm}
-            return json.dumps(combine)
-
-
-    @Validator.isRequired(required=['OrderId', 'Exchange'])
-    @Validator.ValidateInputDataTypes
-
-    def OrderDetails(self, OrderId , Exchange : ExchangeEnum) -> str:
-        """
-
-          Please use this method to retrive the details of single order.
-          Response Fields :
-           - Symbol
-            - Product Type
-            - Order type
-            - Quantity
-            - Price
-            - Validity
-            - Trade ID
-            - Trade Status
-
-        """
-        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
-            LOGGER.info("OrderDetails method is called for MCX/NCDEX.")
-            LOGGER.debug("OrderDetails method is called for MCX/NCDEX.")
-            url = self.__router._OrderDetailsURL_comm().format(userid=self.__constants.coAccId, orderid=OrderId)
-            resp = self.__http._GetMethod(url)
-            LOGGER.debug("Response receieved: %s", resp)
-            return json.dumps(resp)
-        else:
-            LOGGER.info("OrderDetails method is called.")
-            LOGGER.debug("OrderDetails method is called.")
-            url = self.__router._OrderDetailsURL().format(userid=self.__constants.eqAccId, orderid=OrderId)
-            resp = self.__http._GetMethod(url)
-            LOGGER.debug("Response receieved: %s", resp)
-            return json.dumps(resp)
-
-
-    def OrderHistory(self, StartDate, EndDate) -> str:
-        """
-
-          This method will retrive all the historical orders placed from `StartDate` to `EndDate`
-
-          StartDate : Start Date of Search
-
-          EndDate : End Date of search
-
-        """
-        LOGGER.info("OrderHistory method is called.")
-
-        LOGGER.debug("OrderHistory method is called with account type: %s",
-            self.__constants.Data['data']['lgnData']['accTyp'])
-
-        if self.__constants.Data['data']['lgnData']['accTyp'] == 'EQ':
-            url = self.__router._OrderHistoryURL().format(userid=self.__constants.eqAccId, StartDate=StartDate,
-                                                         EndDate=EndDate)
-            rep = self.__http._GetMethod(url)
-            LOGGER.debug("Response receieved: %s", rep)
-            return json.dumps({"eq": rep, "comm": ""})
-
-        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'CO':
-            url = self.__router._OrderHistoryURL_comm().format(userid=self.__constants.coAccId,
-                                                              StartDate=StartDate,
-                                                              EndDate=EndDate)
-            rep = self.__http._GetMethod(url)
-            LOGGER.debug("Response receieved: %s", rep)
-            return json.dumps({"eq": "", "comm": rep})
-
-        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'COMEQ':
-            url = self.__router._OrderHistoryURL().format(userid=self.__constants.eqAccId, StartDate=StartDate,
-                                                         EndDate=EndDate)
-            url_comm = self.__router._OrderHistoryURL_comm().format(userid=self.__constants.coAccId,
-                                                                   StartDate=StartDate,
-                                                                   EndDate=EndDate)
-            rep = self.__http._GetMethod(url)
-            LOGGER.debug("Response receieved for eq: %s", rep)
-            rep_comm = self.__http._GetMethod(url_comm)
-            LOGGER.debug("Response receieved for comm: %s", rep_comm)
-            combine = {"eq": rep, "comm": rep_comm}
-            return json.dumps(combine)
-
-
-    def Holdings(self) -> str:
-        """
-        Holdings comprises of the user's portfolio of long-term equity delivery stocks. An instrument in a holding's portfolio remains there indefinitely until its sold or is delisted or changed by the exchanges. Underneath it all, instruments in the holdings reside in the user's DEMAT account, as settled by exchanges and clearing institutions.
-        """
-        LOGGER.info("Holdings method is called.")
-        LOGGER.debug("Holdings method is called with account type: %s",
-            self.__constants.Data['data']['lgnData']['accTyp'])
-
-        if self.__constants.Data['data']['lgnData']['accTyp'] == 'EQ':
-            url = self.__router._HoldingURL().format(userid=self.__constants.eqAccId)
-            rep = self.__http._GetMethod(url)
-            LOGGER.debug("Response receieved: %s", rep)
-            return json.dumps({"eq": rep, "comm": ""})
-
-        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'CO':
-            # url = self.__config.HoldingURL_comm().format(userid=self.__constants.coAccId)
-            LOGGER.debug("Holdings not available for 'CO' account type.")
-            return json.dumps({"eq": "", "comm": ""})
-
-        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'COMEQ':
-            url = self.__router._HoldingURL().format(userid=self.__constants.eqAccId)
-            # url_comm = self.__config.HoldingURL_comm().format(userid=self.__constants.coAccId)
-            rep = self.__http._GetMethod(url)
-            LOGGER.debug("Response receieved: %s", rep)
-            # rep_comm = self.__http.GetMethod(url_comm)
-            LOGGER.debug("Holdings not available for 'CO' account type.")
-            combine = {"eq": rep, "comm": ""}
-            return json.dumps(combine)
-
-
-    @Validator.isRequired(required=['Trading_Symbol','Exchange','Action','Duration','Order_Type','Quantity','Streaming_Symbol','Limit_Price','TriggerPrice', 'ProductCode'])
-    @Validator.ValidateInputDataTypes
-
-    def PlaceTrade(self, Trading_Symbol, Exchange : ExchangeEnum, Action : ActionEnum, Duration : DurationEnum, Order_Type : OrderTypeEnum, Quantity : int, Streaming_Symbol, Limit_Price, Disclosed_Quantity="0", TriggerPrice="0", ProductCode : ProductCodeENum = ProductCodeENum.CNC) -> str :
-
-        """
-        Order placement refers to the function by which you as a user can place an order to respective exchanges. Order placement allows you to set various parameters like the symbol, action (buy, sell, stop loss buy, stop loss sell), product type, validity period and few other custom parameters and then finally place the order. Any order placed will first go through a risk validation in our internal systems and will then be sent to exchange. Usually any order successfully placed will have OrderID and ExchangeOrderID fields populated. If ExchangeOrderID is blank it usually means that the order has not been sent and accepted at respective exchange.
-
-        Order placement method
-
-        - `Trading_Symbol` : Trading Symbol of the Scrip
-
-        - `Exchange` : Exchange
-
-        - `Action` : BUY/SELL
-
-        - `Duration` : DAY/IOC/EOS(for BSE)
-
-        - `Order_Type`: LIMIT/MARKET/STOP_LIMIT/STOP_MARKET
-
-        - `Quantity` : Quantity of the scrip
-
-        - `Streaming_Symbol` : companycode_exchange to be obtained from Contract file downloaded
-
-        - `Limit_Price` : Limit price of scrip
-
-        - `Disclosed_Quantity` : Quantity to be disclosed while order placement
-
-        - `TriggerPrice` : Trigger Price applicable for SL/SL-M Orders
-
-        - `ProdcutCode` : CNC/MIS/NRML/MTF
-
-        """
-        LOGGER.info("PlaceTrade method is called.")
-
-        data = {'trdSym': Trading_Symbol, 'exc': Exchange.value, 'action': Action.value, 'dur': Duration.value,
-                'ordTyp': Order_Type.value, 'qty': str(Quantity), 'dscQty': Disclosed_Quantity, 'sym': Streaming_Symbol,
-                'mktPro': "",
-                'lmPrc': Limit_Price, 'trgPrc': TriggerPrice, 'prdCode': ProductCode.value, 'posSqr': "N",
-                'minQty': "0", 'ordSrc': "API", 'vnCode': '', 'rmk': '', 'flQty': "0"}
-
-        LOGGER.debug("PlaceTrade method is called with data: %s", data)
-        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
-            url = self.__router._PlaceTradeURL_comm().format(userid=self.__constants.coAccId)
-            reply = self.__http._PostMethod(url, json.dumps(data))
-            LOGGER.debug("Response received for MCX/NCDEX: %s", reply)
-            return json.dumps(reply)
-        else:
-            url = self.__router._PlaceTradeURL().format(userid=self.__constants.eqAccId)
-            reply = self.__http._PostMethod(url, json.dumps(data))
-            LOGGER.debug("Response received: %s", reply)
-            return json.dumps(reply)
-
-
-    @Validator.isRequired(required=['Trading_Symbol','Exchange','Action','Duration','Order_Type','Quantity','Streaming_Symbol','Limit_Price','TriggerPrice', 'ProductCode'])
-    @Validator.ValidateInputDataTypes
-
-    def PlaceCoverTrade(self, Trading_Symbol, Exchange : ExchangeEnum, Action : ActionEnum, Duration : DurationEnum, Order_Type : OrderTypeEnum, Quantity : int, Streaming_Symbol, Limit_Price, Disclosed_Quantity="0", TriggerPrice="0", ProductCode : ProductCodeENum = ProductCodeENum.CNC) -> str or None :
-
-        """
-
-        A Cover Order is an order type for intraday trades. A Cover Order lets you to place trades with very high leverage of up to 20 times the available limits (Cash/Stocks collateral limits)
-
-        Pay a fraction of total order amount (10% or Rs. 20) to own the shares. In case it falls below the following price, sell it off to prevent me losing money from sharp price drops.
-
-        - `Trading_Symbol` : Trading Symbol of the Scrip
-
-        - `Exchange` : Exchange
-
-        - `Action` : BUY/SELL
-
-        - `Duration` : DAY/IOC/EOS(for BSE)
-
-        - `Order_Type`: LIMIT/MARKET/STOP_LIMIT/STOP_MARKET
-
-        - `Quantity` : Quantity of the scrip
-
-        - `Streaming_Symbol` : companycode_exchange to be obtained from Contract file downloaded
-
-        - `Limit_Price` : Limit price of scrip
-
-        - `Disclosed_Quantity` : Quantity to be disclosed while order placement
-
-        - `TriggerPrice` : Trigger Price applicable for SL/SL-M Orders
-
-        - `ProdcutCode` : CNC/MIS/NRML/MTF
-
-        """
-        LOGGER.info("PlaceCoverTrade is method is called.")
-        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
-            print('Operation invalid for Commodities')
-            LOGGER.debug("Operation is disabled for commodities.")
-            return
-
-        data = {'trdSym': Trading_Symbol, 'exc': Exchange, 'action': Action, 'dur': Duration,
-                'ordTyp': Order_Type, 'qty': Quantity, 'dscQty': Disclosed_Quantity, 'sym': Streaming_Symbol,
-                'mktPro': "",
-                'lmPrc': Limit_Price, 'trgPrc': TriggerPrice, 'prdCode': ProductCode, 'posSqr': "false",
-                'minQty': "0", 'ordSrc': "API", 'vnCode': '', 'rmk': '', 'flQty': "0", }
-
-        LOGGER.debug("PlaceCoverTrade method is called with data: %s", data)
-        url = self.__router._PlaceCoverTradeURL().format(userid=self.__constants.eqAccId)
-        resp = self.__http._PostMethod(url, json.dumps(data))
-        LOGGER.debug("Response receieved: %s", resp)
-        return json.dumps(resp)
-
-
-    @Validator.isRequired(required=['Trading_Symbol','Exchange','Action','Duration','Order_Type','Quantity','Limit_Price','TriggerPrice', 'ProductCode', 'DTDays'])
-    @Validator.ValidateInputDataTypes
-
-    def PlaceGtcGtdTrade(self, Trading_Symbol, Exchange : ExchangeEnum, Action : ActionEnum, Duration : DurationEnum, Order_Type : OrderTypeEnum, Quantity : int, streaming_symbol, Limit_Price, Product_Code : ProductCodeENum, DTDays) -> str :
-
-        LOGGER.info("PlaceGtcGtdTrade method is called.")
-
-        data = {'trdSym': Trading_Symbol, 'exc': Exchange, 'action': Action, 'dur': Duration, 'ordTyp': Order_Type,
-                'qty': Quantity, 'lmPrc': Limit_Price, 'prdCode': Product_Code,
-                'dtDays': DTDays, 'ordSrc': 'API', 'vnCode': '', 'oprtn': '<=', 'srcExp': '', 'tgtId': '',
-                'brnchNm': '', 'vlDt': DTDays, 'sym': streaming_symbol,
-                'brk': '', }
-
-        LOGGER.debug("PlaceGtcGtdTrade method is called with data: %s", data)
-        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
-            url = self.__router._PlaceTradeURL_comm().format(userid=self.__constants.coAccId)
-            reply = self.__http._PostMethod(url, json.dumps(data))
-            LOGGER.debug("Response recieved: %s", reply)
-            return json.dumps(reply)
-        else:
-            url = self.__router._PlaceGtcGtdTradeURL().format(userid=self.__constants.eqAccId)
-            reply = self.__http._PostMethod(url, json.dumps(data))
-            LOGGER.debug("Response recieved: %s", reply)
-            return json.dumps(reply)
-
-
-    @Validator.isRequired(required=['Trading_Symbol','Exchange','Action','Duration','Order_Type','Quantity','Limit_Price','Order_ID','TriggerPrice', 'ProductCode'])
-    @Validator.ValidateInputDataTypes
-
-    def ModifyTrade(self, Trading_Symbol, Exchange : ExchangeEnum, Action : ActionEnum, Duration : DurationEnum, Order_Type : OrderTypeEnum, Quantity : int, Streaming_Symbol, Limit_Price, Order_ID, Disclosed_Quantity="0", TriggerPrice="0", ProductCode : ProductCodeENum = ProductCodeENum.CNC) -> str :
-        """
-        Modify orders allows a user to change certain aspects of the order once it is placed. Depending on the execution state of the order (i.e. either completely open, partially open) there are various levels of modification allowed. As a user you can edit the product type, order quantity, order validity and certain other parameters. Please note that any modifications made to an order will be sent back to the risk system for validation before being submitted and there are chances that an already placed order may get rejected in case of a modification.
-
-        Modify Order
-
-        `Trading_Symbol` : Trading Symbol of the Scrip
-
-        `Exchange` : Exchange
-
-        `Action` : BUY/SELL
-
-        `Duration` : DAY/IOC/EOS(for BSE)
-
-        `Order_Type`: LIMIT/MARKET/STOP_LIMIT/STOP_MARKET
-
-        `Quantity` : Quantity of the scrip
-
-        `Streaming_Symbol` : companycode_exchange to be obtained from Contract file downloaded
-
-        `Limit_Price` : Limit price of scrip
-
-        `Disclosed_Quantity` : Quantity to be disclosed while order placement
-
-        `TriggerPrice` : Trigger Price applicable for SL/SL-M Orders
-
-        `ProductCode` : CNC/MIS/NRML/MTF
-
-
-        """
-        LOGGER.info("ModifyTrade method is called.")
-
-        data = {'trdSym': Trading_Symbol, 'exc': Exchange, 'action': Action, 'dur': Duration, 'flQty': "0",
-                'ordTyp': Order_Type, 'qty': Quantity, 'dscQty': Disclosed_Quantity, 'sym': Streaming_Symbol,
-                'mktPro': "",
-                'lmPrc': Limit_Price, 'trgPrc': TriggerPrice, 'prdCode': ProductCode, 'dtDays': '', 'nstOID': Order_ID}
-        LOGGER.debug("ModifyTrade method is called with method: %s", data)
-        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
-            url = self.__router._ModifyTradeURL_comm().format(userid=self.__constants.coAccId)
-            resp = self.__http._PutMethod(url, json.dumps(data))
-            LOGGER.debug("Response recieved: %s", resp)
-            return json.dumps(resp)
-
-        else:
-            url = self.__router._ModifyTradeURL().format(userid=self.__constants.eqAccId)
-            resp = self.__http._PutMethod(url, json.dumps(data))
-            LOGGER.debug("Response recieved: %s", resp)
-            return json.dumps(resp)
-
-
-    @Validator.isRequired(required=['Trading_Symbol','Exchange','Action','Duration','Order_Type','Quantity','Limit_Price','Order_ID','TriggerPrice', 'ProductCode'])
-    @Validator.ValidateInputDataTypes
-
-    def ModifyCoverTrade(self, Trading_Symbol, Exchange : ExchangeEnum, Action : ActionEnum, Duration : DurationEnum, Order_Type : OrderTypeEnum, Quantity : int, Streaming_Symbol, Limit_Price, Order_ID, Disclosed_Quantity="0", TriggerPrice="0", ProductCode : ProductCodeENum = ProductCodeENum.CNC) -> str or None:
-
-        """
-
-        Modify Cover Order
-
-        Trading_Symbol : Trading Symbol of the Scrip
-
-        Exchange : Exchange
-
-        Action : BUY/SELL
-
-        Duration : DAY/IOC/EOS(for BSE)
-
-        Order_Type: LIMIT/MARKET/STOP_LIMIT/STOP_MARKET
-
-        Quantity : Quantity of the scrip
-
-        Streaming_Symbol : companycode_exchange to be obtained from Contract file downloaded
-
-        Limit_Price : Limit price of scrip
-
-        Disclosed_Quantity : Quantity to be disclosed while order placement
-
-        TriggerPrice : Trigger Price applicable for SL/SL-M Orders
-
-        ProductCode : CNC/MIS/NRML/MTF
-
-        """
-        LOGGER.info("ModifyCoverTrade method is called")
-        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
-            print('Operation invalid for Commodities')
-            LOGGER.debug("Operation is blocked for commodities.")
-            return
-
-        data = {'trdSym': Trading_Symbol, 'exc': Exchange, 'action': Action, 'dur': Duration, 'flQty': "0",
-                'ordTyp': Order_Type, 'qty': Quantity, 'dscQty': Disclosed_Quantity, 'sym': Streaming_Symbol,
-                'mktPro': "",
-                'lmPrc': Limit_Price, 'trgPrc': TriggerPrice, 'prdCode': ProductCode, 'dtDays': '', 'nstOID': Order_ID}
-        LOGGER.debug("ModifyCoverTrade method is called with data: %s", data)
-        url = self.__router._ModifyCoverTradeURL().format(userid=self.__constants.eqAccId)
-        resp = self.__http._PutMethod(url, json.dumps(data))
-        LOGGER.debug("Response recieved: %s", resp)
-        return json.dumps(resp)
-
-
-    @Validator.isRequired(required=['Order_ID','Exchange','Order_Type','ProductCode'])
-    @Validator.ValidateInputDataTypes
-
-    def CancelTrade(self, Order_ID, Exchange : ExchangeEnum, Order_Type : OrderTypeEnum, Product_Code : ProductCodeENum) -> str :
-        """
-
-        An order can be cancelled, as long as on order is open or pending in the system
-
-        Cancel Order
-
-        OrderId : Nest OrderId
-
-        """
-        LOGGER.info("CancelTrade method is called.")
-
-        data = {"nstOID": Order_ID, "exc": Exchange, "prdCode": Product_Code, "ordTyp": Order_Type}
-        LOGGER.debug("CancelTrade method is called with data: %s", data)
-        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
-            url = self.__router._CancelTradeURL_comm().format(userid=self.__constants.coAccId)
-            resp = self.__http._PutMethod(url, json.dumps(data))
-            LOGGER.debug("Response recieved: %s", resp)
-            return json.dumps(resp)
-
-        else:
-            url = self.__router._CancelTradeURL().format(userid=self.__constants.eqAccId)
-            resp = self.__http._PutMethod(url, json.dumps(data))
-            LOGGER.debug("Response recieved: %s", resp)
-            return json.dumps(resp)
-
-
-    def MFOrderBook(self, fromDate, toDate) -> str :
-        '''
-
-        This method will retrieve the MF Order Book.
-         fromDate: From Date
-         toDate: To Date
-         :return: MF Order Book
-
-         Typical order book response will be a nested JSON containing below fields
-            - Symbol
-            - Product Type
-            - Order type
-            - Quantity
-            - Price
-            - Validity
-            - Order ID
-            - Order Status
-
-        '''
-        LOGGER.info("MFOrderBook method is called.")
-        url = self.__router._OrderBookMFURL().format(userid=self.__constants.eqAccId, fromDate=fromDate,
-                                                    toDate=toDate)
-        rep = self.__http._GetMethod(url)
-        LOGGER.debug("MFOrderBook method is called. Receieved response: %s", rep)
-        return json.dumps(rep)
-
-
-    @Validator.isRequired(required='Order_ID')
-
-    def ExitCoverTrade(self, Order_ID) -> str :
-        """
-        This functionality allows you to completely exit a cover order which includes cancelling any unplaced orders and also completely squaring off any executed orders. For the orders which were executed it will usually modify the stop loss order leg and place it as a market order to ensure execution, while any non executed quantity order will get cancelled.
-
-       Exit Cover Order
-
-       OrderId : Nest OrderId
-
-        """
-        LOGGER.info("ExitCoverTrade method is called.")
-        url = self.__router._ExitCoverTradeURL().format(userid=self.__constants.eqAccId)
-        resp = self.__http._PutMethod(url, json.dumps({"nstOID": Order_ID}))
-        LOGGER.debug("ExitCoverTrade method is called for nstOID: %s", Order_ID)
-        LOGGER.debug("Response receieved: %s", resp)
-        return json.dumps(resp)
-
-
-    @Validator.isRequired(required=['Order_ID', 'Syom_Id', 'Status'])
-
-    def ExitBracketTrade(self, Order_Id, Syom_Id, Status) -> str :
-        """
-        Similar to Exit Cover order the functionality will ensure that any non executed open order will be cancelled. However for any orders which are executed it will automatically cancel one of the target or stop loss legs and modify the other leg to be placed as a market order. This will ensure that any executed orders will be squared off in position terms.
-
-       Exit Bracket Order
-
-       OrderId : Nest OrderId
-
-       Syom_Id : Syom_Id obtained post placing Bracket Order
-
-       Status: Current Status of the Bracket Order
-
-       """
-        LOGGER.info("ExitBracketTrade method is called.")
-        data = {'nstOrdNo': Order_Id, 'syomID': Syom_Id, 'sts': Status}
-        params = locals()
-        LOGGER.debug("ExitBracketTrade method is called with data: %s", data)
-        url = self.__router._ExitBracketTradeURL().format(userid=self.__constants.eqAccId)
-        resp = self.__http._DeleteMethod(url, json.dumps(data))
-        del (params["self"])
-        LOGGER.debug("Response receieved: %s", resp)
-        return json.dumps(resp)
-
-
-    @Validator.isRequired(required=['Exchange','Streaming_Symbol','Transaction_Type','Quantity','Duration','Limit_Price','Target','StopLoss','Trailing_Stop_Loss', 'Trailing_Stop_Loss_Value'])
-    @Validator.ValidateInputDataTypes
-
-    def PlaceBracketTrade(self, Exchange : ExchangeEnum, Streaming_Symbol, Transaction_Type : ActionEnum, Quantity : int, Duration : DurationEnum, Disclosed_Quantity, Limit_Price, Target, StopLoss, Trailing_Stop_Loss='Y', Trailing_Stop_Loss_Value="1") -> str or None:
-
-        """
-
-        Bracket Order
-
-        Exchange : Exchange
-
-        Transaction_Type : BUY/SELL
-
-        Duration : DAY/IOC/EOS(for BSE)
-
-        Order_Type: LIMIT/MARKET/STOP_LIMIT/STOP_MARKET
-
-        Quantity : Quantity of the scrip
-
-        Streaming_Symbol : companycode_exchange to be obtained from Contract file downloaded
-
-        Limit_Price : Limit price of scrip
-
-        Disclosed_Quantity : Quantity to be disclosed while order placement
-
-        Target : Absolute Target value
-
-        StopLoss :Absolute Stop Loss value
-
-        Trailing_Stop_Loss : Y/N
-
-        Trailing_Stop_Loss_Value : Number
-
-        """
-        LOGGER.info("PlaceBracketTrade method is called.")
-        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
-            print('Operation invalid for Commodities')
-            LOGGER.debug("Operation invalid for commodities.")
-            return
-
-        data = {'exc': Exchange, 'sym': Streaming_Symbol,
-                'trnsTyp': Transaction_Type, 'qty': Quantity, 'dur': Duration, 'dsQty': Disclosed_Quantity,
-                'prc': Limit_Price, 'trdBsdOn': "LTP", 'sqOffBsdOn': 'Absolute', 'sqOffVal': Target,
-                'slBsdOn': 'Absolute', 'slVal': StopLoss, 'trlSl': Trailing_Stop_Loss,
-                'trlSlVal': Trailing_Stop_Loss_Value, 'ordSrc': 'API'}
-        LOGGER.debug("PlaceBracketTrade method is called with data: %s", data)
-        url = self.__router._PlaceBracketTradeURL().format(userid=self.__constants.eqAccId)
-        resp = self.__http._PostMethod(url, json.dumps(data))
-        LOGGER.debug("Response received: %s", resp)
-        return json.dumps(resp)
-
-
-    def PlaceBasketTrade(self, orderlist : Order) -> str :
-        """
-
-        Basket order allows user to place multiple orders at one time. User can place orders for multiple scrips all at once. One just creates multiple orders for same or different securities and club these orders together to be placed in one go. This helps save time.
-
-        orderlist : List of Order to be placed, Refer: Order Class
-
-        """
-        LOGGER.info("PlaceBasketTrade method is called.")
-        isComm = False
-        lst = []
-        for x in orderlist:
-            if x.exc == ExchangeEnum.MCX or x.exc == ExchangeEnum.NCDEX:
-                isComm = True
-                continue
-
-            #//FIXME: Find better implementation for validation in this method, current implimentation is redundant.
-            data = {'trdSym':   Validator.isRequiredv2('TradingSymbol', x.trdSym),
-                    'exc':      Validator.isRequiredv2('Exchange',x.exc),
-                    'action':   Validator.isRequiredv2('Action',x.action),
-                    'dur':      Validator.isRequiredv2('Duration',x.dur),
-                    'ordTyp':   Validator.isRequiredv2('OrderType',x.ordTyp),
-                    'qty':      Validator.isRequiredv2('Quantity',x.qty),
-                    'dscQty':   x.dscQty,
-                    'price':    Validator.isRequiredv2('Price',x.price),
-                    'trgPrc':   Validator.isRequiredv2('TriggerPrice',x.trgPrc),
-                    'prdCode':  Validator.isRequiredv2('ProductCode',x.prdCode),
-                    'vnCode': '',
-                    'rmk': ''}
-            lst.append(data)
-
-        fd = {
-            "ordLst": lst,
-            "ordSrc": "API"
-        }
-        if isComm == True:
-            print('Basket Order not available for Commodity')
-        LOGGER.debug("PlaceBasketTrade method is called with data: %s", fd)
-        url = self.__router._PlaceBasketTradeURL().format(userid=self.__constants.eqAccId)
-        resp = self.__http._PostMethod(url, json.dumps(fd))
-        LOGGER.debug("Response received: %s", resp)
-        return json.dumps(resp)
-
-
-    def Limits(self) -> str :
-        """
-        Limits refers to the cumulative margins available in your account which can be used for trading and investing in various products. Limits is a combination of the free cash you have (i.e. un-utilized cash), cash equivalent securities (usually margin pledged securities), any money which is in transit (T1/T2 day sell transaction values) and others, all of which can be used for placing orders. Usually whenever you place an order in a given asset and product type our risk management system assesses your limits available and then lets the orders go through or blocks the orders. Limits are dynamic in nature and can be influenced by the Mark to Markets in your positions and sometimes even by the LTP of your holdings.
-
-        Get limits
-
-
-        """
-        LOGGER.info("Limits method is called.")
-        LOGGER.debug("Limits method is called for accout type: %s",
-                self.__constants.Data['data']['lgnData']['accTyp'])
-        if self.__constants.Data['data']['lgnData']['accTyp'] == 'EQ':
-            url = self.__router._LimitsURL().format(userid=self.__constants.eqAccId)
-            resp = self.__http._GetMethod(url)
-            LOGGER.debug("Response recevied: %s", resp)
-            return json.dumps({"eq": resp, "comm": ""})
-
-        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'CO':
-            url = self.__router._LimitsURL_comm().format(userid=self.__constants.coAccId)
-            resp = self.__http._GetMethod(url)
-            LOGGER.debug("Response recevied: %s", resp)
-            return json.dumps({"eq": resp, "comm": resp})
-
-        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'COMEQ':
-            url = self.__router._LimitsURL().format(userid=self.__constants.eqAccId)
-            url_comm = self.__router._LimitsURL_comm().format(userid=self.__constants.coAccId)
-            rep = self.__http._GetMethod(url)
-            LOGGER.debug("Response recevied for eq: %s", rep)
-            rep_comm = self.__http._GetMethod(url_comm)
-            LOGGER.debug("Response recevied for comm: %s", rep_comm)
-            combine = {"eq": rep, "comm": rep_comm}
-            return json.dumps(combine)
-
-
-    def GetAMOStatus(self) -> str :
-        """
-
-        Get AMO status
-
-        """
-        LOGGER.info("Limits method is called.")
-        LOGGER.debug("Limits method is called for accout type: %s",
-                self.__constants.Data['data']['lgnData']['accTyp'])
-
-        if self.__constants.Data['data']['lgnData']['accTyp'] == 'EQ':
-            url = self.__router._GetAMOFlag()
-            resp = self.__http._GetMethod(url)
-            LOGGER.debug("Response recevied: %s", resp)
-            return json.dumps({"eq": resp, "comm": ""})
-
-        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'CO':
-            url = self.__router._GetAMOFlag_comm()
-            resp = self.__http._GetMethod(url)
-            LOGGER.debug("Response recevied: %s", resp)
-            return json.dumps({"eq": "", "comm": resp})
-
-        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'COMEQ':
-            url = self.__router._GetAMOFlag()
-            url_comm = self.__router._GetAMOFlag_comm()
-            rep = self.__http._GetMethod(url)
-            LOGGER.debug("Response recevied for eq: %s", rep)
-            rep_comm = self.__http._GetMethod(url_comm)
-            LOGGER.debug("Response recevied for comm: %s", rep_comm)
-            combine = {"eq": rep, "comm": rep_comm}
-            return json.dumps(combine)
-
-
-    @Validator.isRequired(required=['Trading_Symbol','Exchange','Action','Duration','Order_Type','Quantity','Streaming_Symbol','Limit_Price','TriggerPrice', 'ProductCode'])
-    @Validator.ValidateInputDataTypes
-
-    def PlaceAMOTrade(self, Trading_Symbol, Exchange : ExchangeEnum, Action : ActionEnum, Duration : DurationEnum, Order_Type : OrderTypeEnum, Quantity : int, Streaming_Symbol, Limit_Price, Disclosed_Quantity="0", TriggerPrice="0", ProductCode : ProductCodeENum = ProductCodeENum.CNC) -> str :
-
-        """
-        After market order or AMO in short refers to orders which can be placed once the markets or exchanges are closed for trading. You can place AMO post market hours which will result in the order in question being placed automatically by 9:15 AM - 9:30 AM the next business day. AMO orders usually need to be limit orders in order to prevent inadvertent execution in case of adverse price movement in markets at beginning of day. AMO is a useful way to place your orders in case you do not have time to place orders during market hours.
-
-        After Market Order trade
-
-        Trading_Symbol : Trading Symbol of the Scrip
-
-        Exchange : Exchange
-
-        Action : BUY/SELL
-
-        Duration : DAY/IOC/EOS(for BSE)
-
-        Order_Type: LIMIT/MARKET/STOP_LIMIT/STOP_MARKET
-
-        Quantity : Quantity of the scrip
-
-        Streaming_Symbol : companycode_exchange to be obtained from Contract file downloaded
-
-        Limit_Price : Limit price of scrip
-
-        Disclosed_Quantity : Quantity to be disclosed while order placement
-
-        TriggerPrice : Trigger Price applicable for SL/SL-M Orders
-
-        ProductCode : CNC/MIS/NRML/MTF
-
-        """
-        LOGGER.info("PlaceAMOTrade method is called.")
-
-        data = {'trdSym': Trading_Symbol, 'exc': Exchange, 'action': Action, 'dur': Duration, 'flQty': "0",
-                'ordTyp': Order_Type, 'qty': Quantity, 'dscQty': Disclosed_Quantity, 'sym': Streaming_Symbol,
-                'mktPro': "",
-                'lmPrc': Limit_Price, 'trgPrc': TriggerPrice, 'prdCode': ProductCode, 'posSqr': "false",
-                'minQty': "0", 'ordSrc': "API", 'vnCode': '', 'rmk': ''}
-
-        LOGGER.debug("PlaceAMOTrade method is called with data: %s", data)
-        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
-            url = self.__router._PlaceAMOTrade_comm().format(userid=self.__constants.coAccId)
-            resp = self.__http._PostMethod(url, json.dumps(data))
-            LOGGER.debug("Response receieved: %s",resp)
-            return json.dumps(resp)
-
-        else:
-            url = self.__router._PlaceAMOTrade().format(userid=self.__constants.eqAccId)
-            resp = self.__http._PostMethod(url, json.dumps(data))
-            LOGGER.debug("Response receieved: %s",resp)
-            return json.dumps(resp)
-
-
-    @Validator.isRequired(required=['Trading_Symbol','Exchange','Action','Duration','Order_Type','Quantity','Streaming_Symbol','Limit_Price','Order_ID','TriggerPrice', 'ProductCode'])
-    @Validator.ValidateInputDataTypes
-
-    def ModifyAMOTrade(self, Trading_Symbol, Exchange : ExchangeEnum, Action : ActionEnum, Duration : DurationEnum, Order_Type : OrderTypeEnum, Quantity : int, Streaming_Symbol, Limit_Price, Order_ID, Disclosed_Quantity="0", TriggerPrice="0", ProductCode : ProductCodeENum = "CNC") -> str :
-
-        """
-
-        Modify After Market Order
-
-        Trading_Symbol : Trading Symbol of the Scrip
-
-        Exchange : Exchange
-
-        Action : BUY/SELL
-
-        Duration : DAY/IOC/EOS(for BSE)
-
-        Order_Type: LIMIT/MARKET/STOP_LIMIT/STOP_MARKET
-
-        Quantity : Quantity of the scrip
-
-        Streaming_Symbol : companycode_exchange to be obtained from Contract file downloaded
-
-        Limit_Price : Limit price of scrip
-
-        Disclosed_Quantity : Quantity to be disclosed while order placement
-
-        TriggerPrice : Trigger Price applicable for SL/SL-M Orders
-
-        ProductCode : CNC/MIS/NRML/MTF
-
-        """
-        LOGGER.info("ModifyAMOTrade method is called.")
-
-        data = {'trdSym': Trading_Symbol, 'exc': Exchange, 'action': Action, 'dur': Duration, 'flQty': "0",
-                'ordTyp': Order_Type, 'qty': Quantity, 'dscQty': Disclosed_Quantity, 'sym': Streaming_Symbol,
-                'mktPro': "",
-                'lmPrc': Limit_Price, 'trgPrc': TriggerPrice, 'prdCode': ProductCode, 'dtDays': '', 'nstOID': Order_ID}
-        LOGGER.debug("ModifyAMOTrade method is called with data: %s", data)
-
-        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
-            url = self.__router._ModifyAMOTrade_comm().format(userid=self.__constants.coAccId)
-            resp = self.__http._PutMethod(url, json.dumps(data))
-            LOGGER.debug("Response receieved: %s",resp)
-            return json.dumps(resp)
-
-        else:
-            url = self.__router._ModifyAMOTrade().format(userid=self.__constants.eqAccId)
-            resp = self.__http._PutMethod(url, json.dumps(data))
-            LOGGER.debug("Response receieved: %s",resp)
-            return json.dumps(resp)
-
-
-    @Validator.isRequired(required=['Order_ID','Exchange','Order_Type','ProductCode'])
-    @Validator.ValidateInputDataTypes
-
-    def CancelAMOTrade(self, Order_ID, Exchange : ExchangeEnum, Order_Type : OrderTypeEnum, ProductCode : ProductCodeENum) -> str :
-        """
-
-        Cancel After Market Order
-
-        OrderId : Nest Order Id
-
-        """
-        LOGGER.info("CancelAMOTrade method is called.")
-        data = {"nstOID": Order_ID, "exc": Exchange, "prdCode": ProductCode, "ordTyp": Order_Type}
-        LOGGER.debug("CancelAMOTrade method is called with data: %s", data)
-        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
-            url = self.__router._CancelAMOTrade_comm().format(userid=self.__constants.coAccId)
-            resp = self.__http._PutMethod(url, json.dumps(data))
-            LOGGER.debug("Response received: %s", resp)
-            return json.dumps(resp)
-
-        else:
-            url = self.__router._CancelAMOTrade().format(userid=self.__constants.eqAccId)
-            resp = self.__http._PutMethod(url, json.dumps(data))
-            LOGGER.debug("Response received: %s", resp)
-            return json.dumps(resp)
-
-
-    def PositionSquareOff(self, orderlist : Order) -> str :
-        """
-
-        Square off is a term used in intraday and simply means closing all open positions by the end of the trading day
-
-        orderList : List of orders to be Squared Off. Refer : Orders class.
-
-        """
-        lst_eq = []
-        lst_comm = []
-        LOGGER.info("PositionSquareOff method is called.")
-        for x in orderlist:
-
-            if x.exc == ExchangeEnum.MCX or x.exc == "NCDEX":
-            #//FIXME: Find better implementation for validation in this method, current implimentation is redundant.
-                data = {'trdSym':   Validator.isRequiredv2('TradingSymbol', x.trdSym),
-                        'exc':      Validator.isRequiredv2('Exchange', x.exc),
-                        'action':   Validator.isRequiredv2('Action', x.action),
-                        'dur':      Validator.isRequiredv2('Duration', x.dur),
-                        'flQty':    "0",
-                        'ordTyp':   Validator.isRequiredv2('OrderType',x.ordTyp),
-                        'qty':      Validator.isRequiredv2('Quantity', x.qty),
-                        'dscQty':   x.dscQty,
-                        'sym':      Validator.isRequiredv2('StreamingSymbol',x.sym),
-                        'mktPro':   "",
-                        'lmPrc':    Validator.isRequiredv2('Price', x.price),
-                        'trgPrc':   Validator.isRequiredv2('TriggerPrice', x.trgPrc),
-                        'prdCode':  Validator.isRequiredv2('ProductCode', x.prdCode),
-                        'dtDays':   '',
-                        'posSqr':   "true",
-                        'minQty':   "0",
-                        'ordSrc':   "API",
-                        'vnCode':   '',
-                        'rmk':      ''}
-                lst_comm.append(data)
-            else:
-                data = {'trdSym':   Validator.isRequiredv2('TradingSymbol', x.trdSym),
-                        'exc':      Validator.isRequiredv2('Exchange', x.exc),
-                        'action':   Validator.isRequiredv2('Action', x.action),
-                        'dur':      Validator.isRequiredv2('Duration', x.dur),
-                        'flQty':    "0",
-                        'ordTyp':   Validator.isRequiredv2('OrderType',x.ordTyp),
-                        'qty':      Validator.isRequiredv2('Quantity', x.qty),
-                        'dscQty':   x.dscQty,
-                        'sym':      Validator.isRequiredv2('StreamingSymbol',x.sym),
-                        'mktPro':   "",
-                        'lmPrc':    Validator.isRequiredv2('Price', x.price),
-                        'trgPrc':   Validator.isRequiredv2('TriggerPrice', x.trgPrc),
-                        'prdCode':  Validator.isRequiredv2('ProductCode', x.prdCode),
-                        'dtDays':   '',
-                        'posSqr':   "true",
-                        'minQty':   "0",
-                        'ordSrc':   "API",
-                        'vnCode':   '',
-                        'rmk':      ''}
-                lst_eq.append(data)
-
-        resp_eq = ""
-        resp_comm = ""
-
-        if len(lst_eq) > 0:
-            url = self.__router._PositionSqOffURL().format(userid=self.__constants.eqAccId)
-            LOGGER.debug("PositionSquareOff method is called with data: %s.", lst_eq)
-            resp_eq = self.__http._PostMethod(url, json.dumps(lst_eq))
-
-        if len(lst_comm) > 0:
-            url_comm = self.__router._PositionSqOffURL().format(userid=self.__constants.coAccId)
-            LOGGER.debug("PositionSquareOff method is called with data: %s.", lst_comm)
-            resp_comm = self.__http._PostMethod(url_comm, json.dumps(lst_comm))
-
-        resp = {"eq": resp_eq, "comm": resp_comm}
-        LOGGER.debug("Response received: %s", resp)
-        return json.dumps(resp)
-
-
-    @Validator.isRequired(required=['Order_ID','Fill_Id','New_Product_Code','Old_Product_Code','Exchange','Order_Type','Quantity','Streaming_Symbol','Limit_Price','TriggerPrice', 'ProductCode'])
-    @Validator.ValidateInputDataTypes
-
-    def ConvertPosition(self, Order_ID, Fill_Id, New_Product_Code : ProductCodeENum, Old_Product_Code : ProductCodeENum, Exchange : ExchangeEnum, Order_Type : OrderTypeEnum) -> str :
-        """
-
-        Convert Position : converts your holding position from MIS to CNC and vice-versa
-
-        Order_ID : Nest Order id
-
-        Fill_Id : Fill Id of the trade obtained from Trade API
-
-        New_Product_Code: New Product code of the trade
-
-        Old_Product_Code : Existing Product Code of the trade
-
-        """
-        LOGGER.info("ConvertPosition method is called.")
-        data = {'nstOID': Order_ID, 'flID': Fill_Id,
-                'prdCodeCh': New_Product_Code, 'prdCode': Old_Product_Code,
-                'exc': Exchange, 'ordTyp': Order_Type}
-
-        LOGGER.debug("ConvertPosition method is called with data %s",data)
-        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
-            url = self.__router._ConvertPositionURL_comm().format(userid=self.__constants.coAccId)
-            resp = self.__http._PutMethod(url, json.dumps(data))
-            LOGGER.debug("Response receieved: %s", resp)
-            return json.dumps(resp)
-        else:
-            url = self.__router._ConvertPositionURL().format(userid=self.__constants.eqAccId)
-            resp = self.__http._PutMethod(url, json.dumps(data))
-            LOGGER.debug("Response receieved: %s", resp)
-            return json.dumps(resp)
-
-    # MF Methods
-
-
-    @Validator.ValidateInputDataTypes
-
-    def PlaceMF(self, Token, ISIN_Code, Transaction_Type, Client_Code, Quantity, Amount, ReInv_Flag, Folio_Number, Scheme_Name, Start_Date, End_Date, SIP_Frequency, Generate_First_Order_Today, Scheme_Plan, Scheme_Code, Mandate_Id) -> str :
-
-        '''
-
-        Token:
-
-        ISIN_Code:
-
-        Transaction_Type:
-
-        Client_Code:
-
-        Quantity:
-
-        Amount:
-
-        ReInv_Flag:
-
-        Folio_Number:
-
-        Order_Type:
-
-        Scheme_Name:
-
-        Start_Date:
-
-        End_Date:
-
-        SIP_Frequency:
-
-        Generate_First_Order_Today:
-
-        Scheme_Plan:
-
-        Scheme_Code:
-
-
-        '''
-        LOGGER.info("PlaceMF method is called.")
-        data = {'currentOrdSts': '', 'token': Token, 'isin': ISIN_Code, 'txnTyp': Transaction_Type,
-                'clientCode': Client_Code, 'qty': Quantity, 'amt': Amount, 'reInvFlg': ReInv_Flag,
-                'reqstdBy': self.__constants.eqAccId, 'folioNo': Folio_Number,
-                'ordTyp': 'FRESH', 'txnId': '0', 'schemeName': Scheme_Name, 'rmrk': '',
-                'mnRdmFlg': '', 'ordSrc': 'API', 'strtDy': "1", 'strtDt': Start_Date, 'endDt': End_Date,
-                'sipFrq': SIP_Frequency, 'gfot': Generate_First_Order_Today, 'tnr': '999',
-                'mdtId': Mandate_Id, 'sipregno': '', 'siporderno': '',
-                'schemePlan': Scheme_Plan, 'schemeCode': Scheme_Code, 'euinnumber': '', 'dpc': 'Y',
-                'closeAccountFlag': 'N',
-                'kycflag': '1', 'euinflag': 'N', 'physicalFlag': 'D'}
-
-        LOGGER.info("PlaceMF method is called with data: %s.", data)
-        url = self.__router._PlaceMFURL().format(userid=self.__constants.eqAccId)
-        resp = self.__http._PostMethod(url, json.dumps(data))
-        LOGGER.debug("Response received: %s", resp )
-        return json.dumps(resp)
-
-
-    @Validator.ValidateInputDataTypes
-
-    def ModifyMF(self, Token, ISIN_Code, Transaction_Type, Client_Code, Quantity, Amount, ReInv_Flag, Folio_Number, Scheme_Name, Start_Date, End_Date, SIP_Frequency, Generate_First_Order_Today, Scheme_Plan, Scheme_Code, Transaction_Id, Mandate_Id) -> str :
-
-        '''
-
-        certain attributes of a MF order may be modified., as long as on order is open or pending in the system
-
-        Token:
-
-        ISIN_Code:
-
-        Transaction_Type:
-
-        Client_Code:
-
-        Quantity:
-
-        Amount:
-
-        ReInv_Flag:
-
-        Folio_Number:
-
-        Order_Type:
-
-        Scheme_Name:
-
-        Start_Date:
-
-        End_Date:
-
-        SIP_Frequency:
-
-        Generate_First_Order_Today:
-
-        Scheme_Plan:
-
-        Scheme_Code:
-
-
-        '''
-        LOGGER.info("ModifyMF method is called.")
-        data = {'currentOrdSts': 'ACCEPTED', 'token': Token, 'isin': ISIN_Code, 'txnTyp': Transaction_Type,
-                'clientCode': Client_Code, 'qty': Quantity, 'amt': Amount, 'reInvFlg': ReInv_Flag,
-                'reqstdBy': self.__constants.eqAccId, 'folioNo': Folio_Number,
-                'ordTyp': 'MODIFY', 'txnId': Transaction_Id, 'schemeName': Scheme_Name, 'rmrk': '',
-                'mnRdmFlg': '', 'ordSrc': 'API', 'strtDy': "1", 'strtDt': Start_Date, 'endDt': End_Date,
-                'sipFrq': SIP_Frequency, 'gfot': Generate_First_Order_Today, 'tnr': '999',
-                'mdtId': Mandate_Id, 'sipregno': '', 'siporderno': '',
-                'schemePlan': Scheme_Plan, 'schemeCode': Scheme_Code, 'euinnumber': '', 'dpc': 'Y',
-                'closeAccountFlag': 'N',
-                'kycflag': '1', 'euinflag': 'N', 'physicalFlag': 'D'}
-
-        LOGGER.debug("PlaceMF method is called with data: %s.", data)
-        url = self.__router._PlaceMFURL().format(userid=self.__constants.eqAccId)
-        resp = self.__http._PutMethod(url, json.dumps(data))
-        LOGGER.debug("Response received: %s", resp )
-        return json.dumps(resp)
-
-
-    @Validator.ValidateInputDataTypes
-
-    def CancelMF(self, Token, ISIN_Code, Transaction_Type, Client_Code, Quantity, Amount, ReInv_Flag, Folio_Number, Scheme_Name, Start_Date, End_Date, SIP_Frequency, Generate_First_Order_Today, Scheme_Plan, Scheme_Code, Transaction_Id) -> str :
-
-        '''
-
-        Token:
-
-        ISIN_Code:
-
-        Transaction_Type:
-
-        Client_Code:
-
-        Quantity:
-
-        Amount:
-
-        ReInv_Flag:
-
-        Folio_Number:
-
-        Scheme_Name:
-
-        Start_Date:
-
-        End_Date:
-
-        SIP_Frequency:
-
-        Generate_First_Order_Today:
-
-        Scheme_Plan:
-
-        Scheme_Code:
-
-        '''
-        LOGGER.info("CancelMF method is called.")
-        data = {'currentOrdSts': 'ACCEPTED', 'token': Token, 'isin': ISIN_Code, 'txnTyp': Transaction_Type,
-                'clientCode': Client_Code, 'qty': Quantity, 'amt': Amount, 'reInvFlg': ReInv_Flag,
-                'reqstdBy': self.__constants.eqAccId, 'folioNo': Folio_Number,
-                'ordTyp': 'CANCEL', 'txnId': Transaction_Id, 'schemeName': Scheme_Name, 'rmrk': '',
-                'mnRdmFlg': '', 'ordSrc': 'API', 'strtDy': "1", 'strtDt': Start_Date, 'endDt': End_Date,
-                'sipFrq': SIP_Frequency, 'gfot': Generate_First_Order_Today, 'tnr': '999',
-                'mdtId': '', 'sipregno': '', 'siporderno': '',
-                'schemePlan': Scheme_Plan, 'schemeCode': Scheme_Code, 'euinnumber': '', 'dpc': 'Y',
-                'closeAccountFlag': 'N',
-                'kycflag': '1', 'euinflag': 'N', 'physicalFlag': 'D'}
-
-        LOGGER.debug("CancelMF with data %s", data)
-        url = self.__router._CancelMFURL().format(userid=self.__constants.eqAccId)
-        resp = self.__http._PutMethod(url, json.dumps(data))
-        LOGGER.debug("Response recevied: %s", resp)
-        return json.dumps(resp)
-
-
-    def HoldingsMF(self) -> str :
-        LOGGER.info("HoldingsMF method is called.")
-        params = locals()
-        del (params["self"])
-        url = self.__router._HoldingsMFURL().format(userid=self.__constants.eqAccId)
-        resp = self.__http._GetMethod(url)
-        LOGGER.info("HoldingsMF method is called. Response recevied: %s",resp)
-        return json.dumps(resp)
-
-    # Chart methods
-
-    def __getChartDataOfScrip(self, Exchange, AssetType, Streaming_Symbol, Interval, TillDate = None, IncludeContinuousFutures = False) -> str :
-
-        LOGGER.info("Inside __getChartDataOfScrip method.")
-
-        # If asset type is not amongst "FUTCOM", "FUTCUR", "FUTSTK", "FUTIDX", set IncludeContinuousFutures as FALSE
-        if AssetType not in [AssetTypeEnum.FUTCOM, AssetTypeEnum.FUTCUR, AssetTypeEnum.FUTIDX, AssetTypeEnum.FUTIDX]:
-            IncludeContinuousFutures = False
-
-        data = {'chTyp' : "Interval",
-                'conti' : IncludeContinuousFutures,
-                'ltt' : TillDate
-                }
-
-        LOGGER.debug("__getChartDataOfScrip method is called with data: %s", data)
-
-        url = self.__router._ChartsURL().format(interval = Interval, exc = Exchange, aTyp = AssetType, symbol = Streaming_Symbol)
-        reply = self.__http._PostMethod(url, json.dumps(data))
-
-        if reply != "":
-            reply = ChartResponseFormatter(reply).getOHCLResponse()
-            LOGGER.debug("Response received: %s", reply)
-        return json.dumps(reply)
-
-
-    @Validator.isRequired(required=['Exchange', 'AssetType', 'Interval', 'Streaming_Symbol'])
-    @Validator.ValidateInputDataTypes
-
-    def getIntradayChart(self, Exchange : ChartExchangeEnum, AssetType : AssetTypeEnum, Streaming_Symbol, Interval : IntradayIntervalEnum, TillDate = None, IncludeContinuousFutures : bool = False) -> str :
-        """
-        - `Exchange` : Exchange
-        - `AssetType` : AssetType for the chart
-        - `Streaming_Symbol` : Symbol to fetch chart data for. Eg: 11536_NSE, 4963_BSE, -29 etc
-        - `Interval` : interval for Intraday charts
-        - `TillDate` : Charts data to fetch till date (format : yyyy-MM-dd)
-        - `IncludeContinuousFutures` : boolean. True -> If Continous Futures required. Valid only for instruments (Asset Types) - FUTIDX,FUTSTk,FUTCUR,FUTCOM
-        """
-
-        LOGGER.info("getIntradayChart method is called.")
-
-        response = self.__getChartDataOfScrip(Exchange, AssetType, Streaming_Symbol, Interval, TillDate, IncludeContinuousFutures)
-
-        return response
-
-    @Validator.isRequired(required=['Exchange', 'AssetType', 'Interval', 'Streaming_Symbol'])
-    @Validator.ValidateInputDataTypes
-
-    def getEODChart(self, Exchange : ChartExchangeEnum, AssetType : AssetTypeEnum, Streaming_Symbol, Interval : EODIntervalEnum, TillDate = None, IncludeContinuousFutures : bool = False) -> str :
-        """
-        - `Exchange` : Exchange
-        - `AssetType` : AssetType for the chart
-        - `Streaming_Symbol` : Symbol to fetch chart data for. Eg: 11536_NSE, 4963_BSE, -29 etc
-        - `Interval` : interval for EOD charts
-        - `TillDate` : Charts data to fetch till date (format : yyyy-MM-dd)
-        - `IncludeContinuousFutures` : boolean. True -> If Continous Futures required. Valid only for instruments (Asset Types) - FUTIDX,FUTSTk,FUTCUR,FUTCOM
-        """
-
-        LOGGER.info("getEODChart method is called.")
-
-        response = self.__getChartDataOfScrip(Exchange, AssetType, Streaming_Symbol, Interval, TillDate, IncludeContinuousFutures)
-
-        return response
-
-
-    # Live News methods
-
-    def getNewsCategories(self) -> str:
-        LOGGER.info("getNewsCategories method is called")
-        service = LiveNewsService(self.__router, self.__http, self.__constants.Filename)
-        try:
-            response = service._getNewsCategories()
-        except OSError as e:
-            raise e
-        LOGGER.debug(f"getNewsCategories response is : {response}")
-        return response
-
-    @Validator.ValidateInputDataTypes
-    def getLiveNews(self, holdings : bool, category : str = None, searchText : str = None, pageNumber : int = None) -> str :
-        LOGGER.info("getLiveNews method is called")
-
-        service = LiveNewsService(self.__router, self.__http, self.__constants.Filename)
-        try:
-            if holdings:
-                response = service._getHoldingsNews(category, searchText, pageNumber)
-            else:
-                response = service._getGeneralNews(category, searchText, pageNumber)
-        except OSError as e:
-            raise e
-
-        LOGGER.debug(f"getLiveNews response is : {response}")
-        return response
-
-    @Validator.ValidateInputDataTypes
-    def getNewsForResultsAndStocks(self, holdings : bool, searchText : str = None, pageNumber : int = None) -> str :
-        LOGGER.info("getNewsForResultsAndStocks method is called")
-
-
-        service = LiveNewsService(self.__router, self.__http, self.__constants.Filename)
-        try:
-            if holdings:
-                response = service._getHoldingsNews(["Results", "Stocks in News"], searchText, pageNumber)
-            else:
-                response = service._getResultsAndStocksNews(searchText, pageNumber)
-        except OSError as e:
-            raise e
-
-        LOGGER.debug(f"getNewsForResultsAndStocks response is : {response}")
-        return response
-
-    @Validator.isRequired(['symbol'])
-    @Validator.ValidateInputDataTypes
-    def getLatestCorporateActions(self, symbol : str) :
-        LOGGER.info("getLatestCorporateActions method is called")
-
-        service = LiveNewsService(self.__router, self.__http, self.__constants.Filename)
-        response = service._getLatestCorpActionsAPI(symbol)
-
-        LOGGER.debug(f"getLatestCorporateActions response is : {response}")
-        return response
-
-    # Streaming methods
-
-    def initQuotesStreaming(self) :
-        return QuotesFeed(self.__feedObj)
-
-    def initOrdersStreaming(self, acc_id : str, user_id : str) :
-        return OrdersFeed(self.__feedObj, acc_id, user_id)
-
-    def initLiveNewsStreaming(self) :
-        return LiveNewsFeed(self.__feedObj)
-
-    # Watchlist methods
-
-    def getWatchlistGroups(self):
-        LOGGER.info("getWatchlistGroups method is called.")
-        service = WatchlistService(self.__router, self.__http, self.__constants)
-
-        response = service._getWatchlistGroups()
-
-        LOGGER.debug(f'getWatchlistGroups response is : {response}')
-        return response
-
-    @Validator.isRequired(['GroupName'])
-    @Validator.ValidateInputDataTypes
-
-    def getWatchlistScrips(self, GroupName : str):
-        LOGGER.info("getWatchlistScrips method is called.")
-        service = WatchlistService(self.__router, self.__http, self.__constants)
-
-        response = service._getScripsOfGroup(GroupName)
-
-        LOGGER.debug(f'getWatchlistScrips response is : {response}')
-        return response
-
-    @Validator.isRequired(['GroupName', 'Symbols'])
-    @Validator.ValidateInputDataTypes
-
-    def createWatchlistGroup(self, GroupName : str, Symbols : list):
-        LOGGER.info("createWatchlistGroup method is called.")
-        service = WatchlistService(self.__router, self.__http, self.__constants)
-
-        response = service._createGroup(GroupName, Symbols)
-
-        LOGGER.debug(f'createWatchlistGroup response is : {response}')
-        return response
-
-    @Validator.isRequired(['GroupName', 'Symbols'])
-    @Validator.ValidateInputDataTypes
-    def addSymbolsWatchlist(self, GroupName : str, Symbols : list):
-        LOGGER.info("addSymbolsWatchlist method is called.")
-        service = WatchlistService(self.__router, self.__http, self.__constants)
-
-        response = service._addSymbols(GroupName, Symbols)
-
-        LOGGER.debug(f'addSymbolsWatchlist response is : {response}')
-        return response
-
-    @Validator.isRequired(['GroupName', 'Symbols'])
-    @Validator.ValidateInputDataTypes
-    def deleteSymbolsWatchlist(self, GroupName : str, Symbols : list):
-        LOGGER.info("deleteSymbolsWatchlist method is called.")
-        service = WatchlistService(self.__router, self.__http, self.__constants)
-
-        response = service._deleteSymbols(GroupName, Symbols)
-
-        LOGGER.debug(f'deleteSymbolsWatchlist response is : {response}')
-        return response
-
-    @Validator.isRequired(['GroupNames'])
-    @Validator.ValidateInputDataTypes
-    def deleteWatchlistGroups(self, GroupNames : list):
-        LOGGER.info("deleteWatchlistGroups method is called.")
-        service = WatchlistService(self.__router, self.__http, self.__constants)
-
-        response = service._deleteGroups(GroupNames)
-
-        LOGGER.debug(f'deleteWatchlistGroups response is : {response}')
-        return response
-
-    @Validator.isRequired(['GroupName', 'NewGroupName'])
-    @Validator.ValidateInputDataTypes
-    def renameWatchlistGroup(self, GroupName : str, NewGroupName : str):
-        LOGGER.info("renameWatchlistGroup method is called.")
-        service = WatchlistService(self.__router, self.__http, self.__constants)
-
-        response = service._renameGroup(GroupName, NewGroupName)
-
-        LOGGER.debug(f'renameWatchlistGroup response is : {response}')
-        return response
-
-
-    # Research calls methods
-
-    @Validator.isRequired(["Segment", "Term"])
-    @Validator.ValidateInputDataTypes
-
-    def getActiveResearchCalls(self, Segment : SegmentEnum, Term : TermEnum, MarketCap : MarketCapEnum = None) :
-        LOGGER.info("getActiveResearchCalls method is called.")
-
-        if MarketCap and Segment != "EQ":
-            raise ValidationException("Market Cap is only applicable for EQ segment type. Please try again.")
-
-        service = ResearchCallsService(self.__router, self.__http)
-        response = service._getActiveResearchCalls(Segment, Term, MarketCap)
-        LOGGER.debug(f'getActiveResearchCalls response is : {response}')
-        return response
-
-
-    @Validator.isRequired(["Segment", "Term"])
-    @Validator.ValidateInputDataTypes
-
-    def getClosedResearchCalls(self, Segment : SegmentEnum, Term : TermEnum, Action : ActionEnum = None, FromDate : str = None, ToDate : str = None, RecommendationType : str = None, MarketCap : MarketCapEnum = None) :
-        LOGGER.info("getClosedResearchCalls method is called.")
-
-        if FromDate :
-            Validator.validate_datetime_format(FromDate, r"%Y-%m-%d")
-        if ToDate :
-            Validator.validate_datetime_format(ToDate, r"%Y-%m-%d")
-
-        if MarketCap and Segment != "EQ":
-            raise ValidationException("Market Cap is only applicable for EQ segment type. Please try again.")
-
-        service = ResearchCallsService(self.__router, self.__http)
-        response = service._getClosedResearchCalls(Segment, Term, Action, FromDate, ToDate, RecommendationType, MarketCap)
-        LOGGER.debug(f'getClosedResearchCalls response is : {response}')
-        return response
-
-
-    # Login methods
-
-    def Logout(self) -> None:
-        LOGGER.info("Logout method called.")
-        LOGGER.debug("Logout method called with account type: %s",
-            self.__constants.Data['data']['lgnData']['accTyp'])
-        params = locals()
-        del (params["self"])
-        if self.__constants.Data['data']['lgnData']['accTyp'] == 'EQ':
-            url = self.__router._LogoutURL().format(userid=self.__constants.eqAccId)
-            rep = self.__http._PutMethod(url, {})
-
-        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'CO':
-            url = self.__router._LogoutURL().format(userid=self.__constants.coAccId)
-            rep = self.__http._PutMethod(url, {})
-
-        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'COMEQ':
-            url = self.__router._LogoutURL().format(userid=self.__constants.eqAccId)
-            rep = self.__http._PutMethod(url, {})
-
-        if rep != "":
-            if path.exists(self.__filename):
-                LOGGER.debug("File with account related details is removed.")
-                os.remove(self.__filename)
+import configparser
+import errno
+import json
+import logging
+import os
+from os import path
+from typing import List
+
+from APIConnect.api_constants import ApiConstants
+from APIConnect.api_utils import ApiUtils
+from APIConnect.http import Http, init_proxies
+from APIConnect.login_helper import LoginHelper
+from APIConnect.order import Order
+from APIConnect.validator import Validator
+from constants.action import ActionEnum
+from constants.asset_type import AssetTypeEnum
+from constants.chart_exchange import ChartExchangeEnum
+from constants.duration import DurationEnum
+from constants.eod_Interval import EODIntervalEnum
+from constants.exchange import ExchangeEnum
+from constants.intraday_interval import IntradayIntervalEnum
+from constants.order_type import OrderTypeEnum
+from constants.product_code import ProductCodeENum
+from constants.router import Router
+from feed.feed import Feed
+from feed.livenews_feed import LiveNewsFeed
+from feed.orders_feed import OrdersFeed
+from feed.quotes_feed import QuotesFeed
+from resources.chart_response_formatter import ChartResponseFormatter
+from services.live_news_service import LiveNewsService
+from services.watchlist_service import WatchlistService
+
+logging.basicConfig(filename = 'apiconnect.log',
+        level=logging.DEBUG,
+        format="%(asctime)s [%(levelname)s] %(name)s: %(message)s")
+LOGGER = logging.getLogger(__name__)
+
+LOG_LEVELS = {
+    'INFO': logging.INFO,
+    'DEBUG': logging.DEBUG,
+    'ERROR': logging.ERROR,
+    'CRITICAL': logging.CRITICAL
+}
+
+def init_logger(conf) -> None:
+    """
+    Method to initialize logger configuration via provided configuration object.
+    - Parameters:\n
+    `conf`: ConfigParser object of provided settings.ini file.
+    """
+
+    LOG_LEVEL=None
+    LOG_FILE=None
+    if 'LOG_LEVEL' in conf['GLOBAL'] and conf['GLOBAL']['LOG_LEVEL'] in LOG_LEVELS:
+        LOG_LEVEL = LOG_LEVELS[conf['GLOBAL']['LOG_LEVEL']]
+    if 'LOG_FILE' in conf['GLOBAL']:
+        LOG_FILE = conf['GLOBAL']['LOG_FILE']
+    if LOG_FILE or LOG_LEVEL:
+        for handler in logging.root.handlers[:]:
+            logging.root.removeHandler(handler)
+        LOG_FILE = LOG_FILE if LOG_FILE else 'apiconnect.log'
+        LOG_LEVEL = LOG_LEVEL if LOG_LEVEL else logging.INFO
+        logging.basicConfig(filename=LOG_FILE, level=LOG_LEVEL,
+                format="%(asctime)s [%(levelname)s] %(name)s: %(message)s")
+
+class APIConnect:
+
+    def __init__(self, ApiKey, Password, reqID, downloadContract: bool, conf = None) -> None:
+        self.__conf = None
+        self.__init_logger = init_logger
+        if conf:
+            self.__conf = configparser.ConfigParser()
+            try:
+                if path.exists(conf):
+                    self.__conf.read(conf)
+                    self.__init_logger(self.__conf)
+                    LOGGER.info("Loggers initiated with provided configuration.")
+                else:
+                    raise FileNotFoundError(
+                        errno.ENOENT, os.strerror(errno.ENOENT), conf)
+            except Exception as ex:
+                LOGGER.exception("Error occurred while parsing provided configuaration file: %s", ex)
+                raise ex
+        else:
+            LOGGER.info("Logger initiated with default values.")
+
+        self.__version = '2.0.2'
+        self.__dc = downloadContract
+        self.__filename = "data_" + ApiKey + '.txt'
+        self.__router = Router(self.__conf)
+        self.__constants = ApiConstants()
+        self.__init_proxies = init_proxies
+        self.__proxies = self.__init_proxies(self.__conf)
+        self.__http = Http(self.__constants, self.__proxies)
+        self.__constants.Filename = self.__filename
+        self.__constants.ApiKey = ApiKey
+        self.__login_helper = LoginHelper(self.__http, self.__router, self.__constants, self.__proxies)
+        self.__api_utils = ApiUtils(self.__version, self.__http, self.__router, self.__constants)
+        AppIdKey = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhcHAiOjAsImZmIjoiVyIsImJkIjoid2ViLXBjIiwibmJmIjoxNjg0NTAwMDU0LCJzcmMiOiJlbXRtdyIsImF2IjoiMi4wLjIiLCJhcHBpZCI6ImM0YTFmYjE1Yjk2Y2E5OGRiOWVkOTVkNmFkZmJlOWM2IiwiaXNzIjoiZW10IiwiZXhwIjoxNjg0NTIxMDAwLCJpYXQiOjE2ODQ1MDAzNTR9.XuH-LuW3STn15EjZNmh31ZqNUsl98r_8aIJfmJ_CapE"
+
+        if conf and self.__conf['GLOBAL'].get('AppIdKey'):
+            AppIdKey = self.__conf['GLOBAL'].get('AppIdKey')
+        self.__constants.AppIdKey = AppIdKey
+
+        if path.exists(self.__filename):
+            LOGGER.info("User data file found, loading data.")
+            read = open(self.__filename, 'r').read()
+            j = json.loads(read)
+            self.__constants.VendorSession = j['vt']
+            self.__constants.JSessionId =  j['auth']
+            self.__constants.eqAccId = j['eqaccid']
+            self.__constants.coAccId = j['coaccid']
+            self.__constants.Data = j['data']
+            self.__constants.ProfileId = j.get('data').get('data').get('lgnData').get('accs').get('prfId')
+            self.__constants.AppIdKey = j['appidkey']
+        else:
+            self.__login_helper._GenerateVendorSession(ApiKey, Password)
+            self.__login_helper._GetAuthorization(reqID)
+
+        self.__api_utils._setProductCodes()
+
+        self.__feedObj = Feed(self.__conf)
+
+        self.__api_utils._CheckUpdate()
+
+        self.__login_helper._Instruments(self.__dc, self.__proxies)
+
+
+    def GetLoginData(self) -> str:
+        """
+
+        Get Login Info.
+
+        """
+        return json.dumps(self.__constants.Data)
+
+# Trade Methods
+
+    def OrderBook(self) -> str:
+        """
+
+        This method will retrieve the equity Order Book. Typical order book response will be a nested JSON containing below fields
+            - Symbol
+            - Product Type
+            - Order type
+            - Quantity
+            - Price
+            - Validity
+            - Order ID
+            - Order Status
+
+        """
+        LOGGER.info("OrderBook method is called.")
+        if self.__constants.Data['data']['lgnData']['accTyp'] == 'EQ':
+            url = self.__router._OrderBookURL().format(userid=self.__constants.eqAccId)
+            LOGGER.debug("OrderBook method is called for 'EQ' account type")
+            eq = self.__http._GetMethod(url)
+            LOGGER.debug("Response received: %s", eq)
+            return json.dumps({"eq": eq, "comm": ""})
+
+        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'CO':
+            url = self.__router._OrderBookURL_comm().format(userid=self.__constants.coAccId, reqtype='COMFNO')
+            LOGGER.debug("OrderBook method is called for 'CO' account type")
+            comm = self.__http._GetMethod(url)
+            LOGGER.debug("Response received: %s", comm)
+            return json.dumps({"eq": "", "comm": comm})
+
+        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'COMEQ':
+            url = self.__router._OrderBookURL().format(userid=self.__constants.eqAccId)
+            LOGGER.debug("OrderBook method is called for 'COMEQ' account type")
+            url_comm = self.__router._OrderBookURL_comm().format(userid=self.__constants.coAccId, reqtype='COMFNO')
+            rep = self.__http._GetMethod(url)
+            LOGGER.debug("Response for eq: %s", rep)
+            rep_comm = self.__http._GetMethod(url_comm)
+            LOGGER.debug("Response for comm: %s", rep_comm)
+            combine = {"eq": rep, "comm": rep_comm}
+            return json.dumps(combine)
+
+
+    def TradeBook(self) -> str:
+
+        """
+
+          This method will retrieve the Trade Book. Typical trade book response will be a nested JSON containing below fields
+            - Symbol
+            - Product Type
+            - Order type
+            - Quantity
+            - Price
+            - Validity
+            - Trade ID
+            - Trade Status
+
+        """
+        LOGGER.info("TradeBook method is called.")
+        if self.__constants.Data['data']['lgnData']['accTyp'] == 'EQ':
+            url = self.__router._TradeBookURL().format(userid=self.__constants.eqAccId)
+            # return json.dumps({"eq": self.__http.GetMethod(url), "comm": ""})
+            LOGGER.debug("TradeBook method is called for 'EQ' account type")
+            eq = self.__http._GetMethod(url)
+            LOGGER.debug("Response received: %s", eq)
+            return json.dumps({"eq": eq, "comm": ""})
+
+        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'CO':
+            url = self.__router._TradeBookURL_comm().format(userid=self.__constants.coAccId)
+            # return json.dumps({"eq": "", "comm": self.__http.GetMethod(url)})
+            LOGGER.debug("TradeBook method is called for 'CO' account type")
+            comm = self.__http._GetMethod(url)
+            LOGGER.debug("Response received: %s", comm)
+            return json.dumps({"eq": "", "comm": comm})
+
+        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'COMEQ':
+            url = self.__router._TradeBookURL().format(userid=self.__constants.eqAccId)
+            url_comm = self.__router._TradeBookURL_comm().format(userid=self.__constants.coAccId)
+            LOGGER.debug("TradeBook method is called for 'COMEQ' account type")
+            rep = self.__http._GetMethod(url)
+            LOGGER.debug("Response for eq: %s", rep)
+            rep_comm = self.__http._GetMethod(url_comm)
+            LOGGER.debug("Response for comm: %s", rep_comm)
+            combine = {"eq": rep, "comm": rep_comm}
+            return json.dumps(combine)
+
+
+    def NetPosition(self) -> str:
+        """
+        Net position usually is referred to in context of trades placed during the day in case of Equity, or can refer to carry forward positions in case of Derivatives, Currency and Commodity. It indicates the net obligation (either buy or sell) for the given day in a given symbol. Usually you monitor the net positions screen to track the profit or loss made from the given trades and will have options to square off your entire position and book the entire profit and loss.
+
+
+       This method will retrieve the Net position. Typical trade book response will be a nested JSON containing below fields
+            - Symbol
+            - Product Type
+            - Order type
+            - Quantity
+            - Price
+            - Validity
+            - Trade ID
+            - Trade Status
+
+          """
+        LOGGER.info("NetPosition method is called.")
+        if self.__constants.Data['data']['lgnData']['accTyp'] == 'EQ':
+            url = self.__router._NetPositionURL().format(userid=self.__constants.eqAccId)
+            # return json.dumps({"eq": self.__http.GetMethod(url), "comm": ""})
+            LOGGER.debug("NetPosition method is called for 'EQ' account type")
+            eq = self.__http._GetMethod(url)
+            LOGGER.debug("Response received: %s", eq)
+            return json.dumps({"eq": eq, "comm": ""})
+
+        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'CO':
+            url = self.__router._NetPositionURL_comm().format(userid=self.__constants.coAccId)
+            # return json.dumps({"eq": "", "comm": self.__http.GetMethod(url)})
+            LOGGER.debug("NetPosition method is called for 'CO' account type")
+            comm = self.__http._GetMethod(url)
+            LOGGER.debug("Response received: %s", comm)
+            return json.dumps({"eq": "", "comm": comm})
+
+        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'COMEQ':
+            url = self.__router._NetPositionURL().format(userid=self.__constants.eqAccId)
+            url_comm = self.__router._NetPositionURL_comm().format(userid=self.__constants.coAccId)
+            LOGGER.debug("TradeBook method is called for 'COMEQ' account type")
+            rep = self.__http._GetMethod(url)
+            LOGGER.debug("Response for eq: %s", rep)
+            rep_comm = self.__http._GetMethod(url_comm)
+            LOGGER.debug("Response for comm: %s", rep_comm)
+            combine = {"eq": rep, "comm": rep_comm}
+            return json.dumps(combine)
+
+
+    @Validator.isRequired(required=['OrderId', 'Exchange'])
+    @Validator.ValidateInputDataTypes
+
+    def OrderDetails(self, OrderId , Exchange : ExchangeEnum) -> str:
+        """
+
+          Please use this method to retrive the details of single order.
+          Response Fields :
+           - Symbol
+            - Product Type
+            - Order type
+            - Quantity
+            - Price
+            - Validity
+            - Trade ID
+            - Trade Status
+
+        """
+        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
+            LOGGER.info("OrderDetails method is called for MCX/NCDEX.")
+            LOGGER.debug("OrderDetails method is called for MCX/NCDEX.")
+            url = self.__router._OrderDetailsURL_comm().format(userid=self.__constants.coAccId, orderid=OrderId)
+            resp = self.__http._GetMethod(url)
+            LOGGER.debug("Response receieved: %s", resp)
+            return json.dumps(resp)
+        else:
+            LOGGER.info("OrderDetails method is called.")
+            LOGGER.debug("OrderDetails method is called.")
+            url = self.__router._OrderDetailsURL().format(userid=self.__constants.eqAccId, orderid=OrderId)
+            resp = self.__http._GetMethod(url)
+            LOGGER.debug("Response receieved: %s", resp)
+            return json.dumps(resp)
+
+
+    def OrderHistory(self, StartDate, EndDate) -> str:
+        """
+
+          This method will retrive all the historical orders placed from `StartDate` to `EndDate`
+
+          StartDate : Start Date of Search
+
+          EndDate : End Date of search
+
+        """
+        LOGGER.info("OrderHistory method is called.")
+
+        LOGGER.debug("OrderHistory method is called with account type: %s",
+            self.__constants.Data['data']['lgnData']['accTyp'])
+
+        if self.__constants.Data['data']['lgnData']['accTyp'] == 'EQ':
+            url = self.__router._OrderHistoryURL().format(userid=self.__constants.eqAccId, StartDate=StartDate,
+                                                         EndDate=EndDate)
+            rep = self.__http._GetMethod(url)
+            LOGGER.debug("Response receieved: %s", rep)
+            return json.dumps({"eq": rep, "comm": ""})
+
+        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'CO':
+            url = self.__router._OrderHistoryURL_comm().format(userid=self.__constants.coAccId,
+                                                              StartDate=StartDate,
+                                                              EndDate=EndDate)
+            rep = self.__http._GetMethod(url)
+            LOGGER.debug("Response receieved: %s", rep)
+            return json.dumps({"eq": "", "comm": rep})
+
+        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'COMEQ':
+            url = self.__router._OrderHistoryURL().format(userid=self.__constants.eqAccId, StartDate=StartDate,
+                                                         EndDate=EndDate)
+            url_comm = self.__router._OrderHistoryURL_comm().format(userid=self.__constants.coAccId,
+                                                                   StartDate=StartDate,
+                                                                   EndDate=EndDate)
+            rep = self.__http._GetMethod(url)
+            LOGGER.debug("Response receieved for eq: %s", rep)
+            rep_comm = self.__http._GetMethod(url_comm)
+            LOGGER.debug("Response receieved for comm: %s", rep_comm)
+            combine = {"eq": rep, "comm": rep_comm}
+            return json.dumps(combine)
+
+
+    def Holdings(self) -> str:
+        """
+        Holdings comprises of the user's portfolio of long-term equity delivery stocks. An instrument in a holding's portfolio remains there indefinitely until its sold or is delisted or changed by the exchanges. Underneath it all, instruments in the holdings reside in the user's DEMAT account, as settled by exchanges and clearing institutions.
+        """
+        LOGGER.info("Holdings method is called.")
+        LOGGER.debug("Holdings method is called with account type: %s",
+            self.__constants.Data['data']['lgnData']['accTyp'])
+
+        if self.__constants.Data['data']['lgnData']['accTyp'] == 'EQ':
+            url = self.__router._HoldingURL().format(userid=self.__constants.eqAccId)
+            rep = self.__http._GetMethod(url)
+            LOGGER.debug("Response receieved: %s", rep)
+            return json.dumps({"eq": rep, "comm": ""})
+
+        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'CO':
+            # url = self.__config.HoldingURL_comm().format(userid=self.__constants.coAccId)
+            LOGGER.debug("Holdings not available for 'CO' account type.")
+            return json.dumps({"eq": "", "comm": ""})
+
+        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'COMEQ':
+            url = self.__router._HoldingURL().format(userid=self.__constants.eqAccId)
+            # url_comm = self.__config.HoldingURL_comm().format(userid=self.__constants.coAccId)
+            rep = self.__http._GetMethod(url)
+            LOGGER.debug("Response receieved: %s", rep)
+            # rep_comm = self.__http.GetMethod(url_comm)
+            LOGGER.debug("Holdings not available for 'CO' account type.")
+            combine = {"eq": rep, "comm": ""}
+            return json.dumps(combine)
+
+
+    @Validator.isRequired(required=['Trading_Symbol','Exchange','Action','Duration','Order_Type','Quantity','Streaming_Symbol','Limit_Price','TriggerPrice', 'ProductCode'])
+    @Validator.ValidateInputDataTypes
+
+    def PlaceTrade(self, Trading_Symbol, Exchange : ExchangeEnum, Action : ActionEnum, Duration : DurationEnum, Order_Type : OrderTypeEnum, Quantity : int, Streaming_Symbol, Limit_Price, Disclosed_Quantity="0", TriggerPrice="0", ProductCode : ProductCodeENum = ProductCodeENum.CNC) -> str :
+
+        """
+        Order placement refers to the function by which you as a user can place an order to respective exchanges. Order placement allows you to set various parameters like the symbol, action (buy, sell, stop loss buy, stop loss sell), product type, validity period and few other custom parameters and then finally place the order. Any order placed will first go through a risk validation in our internal systems and will then be sent to exchange. Usually any order successfully placed will have OrderID and ExchangeOrderID fields populated. If ExchangeOrderID is blank it usually means that the order has not been sent and accepted at respective exchange.
+
+        Order placement method
+
+        - `Trading_Symbol` : Trading Symbol of the Scrip
+
+        - `Exchange` : Exchange
+
+        - `Action` : BUY/SELL
+
+        - `Duration` : DAY/IOC/EOS(for BSE)
+
+        - `Order_Type`: LIMIT/MARKET/STOP_LIMIT/STOP_MARKET
+
+        - `Quantity` : Quantity of the scrip
+
+        - `Streaming_Symbol` : companycode_exchange to be obtained from Contract file downloaded
+
+        - `Limit_Price` : Limit price of scrip
+
+        - `Disclosed_Quantity` : Quantity to be disclosed while order placement
+
+        - `TriggerPrice` : Trigger Price applicable for SL/SL-M Orders
+
+        - `ProdcutCode` : CNC/MIS/NRML/MTF
+
+        """
+        LOGGER.info("PlaceTrade method is called.")
+
+        data = {'trdSym': Trading_Symbol, 'exc': Exchange.value, 'action': Action.value, 'dur': Duration.value,
+                'ordTyp': Order_Type.value, 'qty': str(Quantity), 'dscQty': Disclosed_Quantity, 'sym': Streaming_Symbol,
+                'mktPro': "",
+                'lmPrc': Limit_Price, 'trgPrc': TriggerPrice, 'prdCode': Validator.product_code(ProductCode.value, Exchange.value, self.__constants.ProductCodesMap), 'posSqr': "N",
+                'minQty': "0", 'ordSrc': "API", 'vnCode': '', 'rmk': '', 'flQty': "0"}
+
+        LOGGER.debug("PlaceTrade method is called with data: %s", data)
+        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
+            url = self.__router._PlaceTradeURL_comm().format(userid=self.__constants.coAccId)
+            reply = self.__http._PostMethod(url, json.dumps(data))
+            LOGGER.debug("Response received for MCX/NCDEX: %s", reply)
+            return json.dumps(reply)
+        else:
+            url = self.__router._PlaceTradeURL().format(userid=self.__constants.eqAccId)
+            reply = self.__http._PostMethod(url, json.dumps(data))
+            LOGGER.debug("Response received: %s", reply)
+            return json.dumps(reply)
+
+
+    @Validator.isRequired(required=['Trading_Symbol','Exchange','Action','Duration','Order_Type','Quantity','Limit_Price','TriggerPrice', 'ProductCode', 'DTDays'])
+    @Validator.ValidateInputDataTypes
+
+    def PlaceGtcGtdTrade(self, Trading_Symbol, Exchange : ExchangeEnum, Action : ActionEnum, Duration : DurationEnum, Order_Type : OrderTypeEnum, Quantity : int, streaming_symbol, Limit_Price, Product_Code : ProductCodeENum, DTDays) -> str :
+
+        LOGGER.info("PlaceGtcGtdTrade method is called.")
+
+        data = {'trdSym': Trading_Symbol, 'exc': Exchange, 'action': Action, 'dur': Duration, 'ordTyp': Order_Type,
+                'qty': Quantity, 'lmPrc': Limit_Price, 'prdCode': Validator.product_code(Product_Code.value, Exchange.value, self.__constants.ProductCodesMap),
+                'dtDays': DTDays, 'ordSrc': 'API', 'vnCode': '', 'oprtn': '<=', 'srcExp': '', 'tgtId': '',
+                'brnchNm': '', 'vlDt': DTDays, 'sym': streaming_symbol,
+                'brk': '', }
+
+        LOGGER.debug("PlaceGtcGtdTrade method is called with data: %s", data)
+        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
+            url = self.__router._PlaceTradeURL_comm().format(userid=self.__constants.coAccId)
+            reply = self.__http._PostMethod(url, json.dumps(data))
+            LOGGER.debug("Response recieved: %s", reply)
+            return json.dumps(reply)
+        else:
+            url = self.__router._PlaceGtcGtdTradeURL().format(userid=self.__constants.eqAccId)
+            reply = self.__http._PostMethod(url, json.dumps(data))
+            LOGGER.debug("Response recieved: %s", reply)
+            return json.dumps(reply)
+
+
+    @Validator.isRequired(required=['Trading_Symbol','Exchange','Action','Duration','Order_Type','Quantity','Limit_Price','Order_ID','TriggerPrice', 'ProductCode'])
+    @Validator.ValidateInputDataTypes
+
+    def ModifyTrade(self, Trading_Symbol, Exchange : ExchangeEnum, Action : ActionEnum, Duration : DurationEnum, Order_Type : OrderTypeEnum, Quantity : int, Streaming_Symbol, Limit_Price, Order_ID, Disclosed_Quantity="0", TriggerPrice="0", ProductCode : ProductCodeENum = ProductCodeENum.CNC) -> str :
+        """
+        Modify orders allows a user to change certain aspects of the order once it is placed. Depending on the execution state of the order (i.e. either completely open, partially open) there are various levels of modification allowed. As a user you can edit the product type, order quantity, order validity and certain other parameters. Please note that any modifications made to an order will be sent back to the risk system for validation before being submitted and there are chances that an already placed order may get rejected in case of a modification.
+
+        Modify Order
+
+        `Trading_Symbol` : Trading Symbol of the Scrip
+
+        `Exchange` : Exchange
+
+        `Action` : BUY/SELL
+
+        `Duration` : DAY/IOC/EOS(for BSE)
+
+        `Order_Type`: LIMIT/MARKET/STOP_LIMIT/STOP_MARKET
+
+        `Quantity` : Quantity of the scrip
+
+        `Streaming_Symbol` : companycode_exchange to be obtained from Contract file downloaded
+
+        `Limit_Price` : Limit price of scrip
+
+        `Disclosed_Quantity` : Quantity to be disclosed while order placement
+
+        `TriggerPrice` : Trigger Price applicable for SL/SL-M Orders
+
+        `ProductCode` : CNC/MIS/NRML/MTF
+
+
+        """
+        LOGGER.info("ModifyTrade method is called.")
+
+        data = {'trdSym': Trading_Symbol, 'exc': Exchange, 'action': Action, 'dur': Duration, 'flQty': "0",
+                'ordTyp': Order_Type, 'qty': Quantity, 'dscQty': Disclosed_Quantity, 'sym': Streaming_Symbol,
+                'mktPro': "",
+                'lmPrc': Limit_Price, 'trgPrc': TriggerPrice, 'prdCode': Validator.product_code(ProductCode.value, Exchange.value, self.__constants.ProductCodesMap), 'dtDays': '', 'nstOID': Order_ID}
+        LOGGER.debug("ModifyTrade method is called with method: %s", data)
+        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
+            url = self.__router._ModifyTradeURL_comm().format(userid=self.__constants.coAccId)
+            resp = self.__http._PutMethod(url, json.dumps(data))
+            LOGGER.debug("Response recieved: %s", resp)
+            return json.dumps(resp)
+
+        else:
+            url = self.__router._ModifyTradeURL().format(userid=self.__constants.eqAccId)
+            resp = self.__http._PutMethod(url, json.dumps(data))
+            LOGGER.debug("Response recieved: %s", resp)
+            return json.dumps(resp)
+
+
+    @Validator.isRequired(required=['Order_ID','Exchange','Order_Type','ProductCode'])
+    @Validator.ValidateInputDataTypes
+
+    def CancelTrade(self, Order_ID, Exchange : ExchangeEnum, Order_Type : OrderTypeEnum, Product_Code : ProductCodeENum) -> str :
+        """
+
+        An order can be cancelled, as long as on order is open or pending in the system
+
+        Cancel Order
+
+        OrderId : Nest OrderId
+
+        """
+        LOGGER.info("CancelTrade method is called.")
+
+        data = {"nstOID": Order_ID, "exc": Exchange, "prdCode": Validator.product_code(Product_Code.value, Exchange.value, self.__constants.ProductCodesMap), "ordTyp": Order_Type}
+        LOGGER.debug("CancelTrade method is called with data: %s", data)
+        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
+            url = self.__router._CancelTradeURL_comm().format(userid=self.__constants.coAccId)
+            resp = self.__http._PutMethod(url, json.dumps(data))
+            LOGGER.debug("Response recieved: %s", resp)
+            return json.dumps(resp)
+
+        else:
+            url = self.__router._CancelTradeURL().format(userid=self.__constants.eqAccId)
+            resp = self.__http._PutMethod(url, json.dumps(data))
+            LOGGER.debug("Response recieved: %s", resp)
+            return json.dumps(resp)
+
+
+    def MFOrderBook(self, fromDate, toDate) -> str :
+        '''
+
+        This method will retrieve the MF Order Book.
+         fromDate: From Date
+         toDate: To Date
+         :return: MF Order Book
+
+         Typical order book response will be a nested JSON containing below fields
+            - Symbol
+            - Product Type
+            - Order type
+            - Quantity
+            - Price
+            - Validity
+            - Order ID
+            - Order Status
+
+        '''
+        LOGGER.info("MFOrderBook method is called.")
+        url = self.__router._OrderBookMFURL().format(userid=self.__constants.eqAccId, fromDate=fromDate,
+                                                    toDate=toDate)
+        rep = self.__http._GetMethod(url)
+        LOGGER.debug("MFOrderBook method is called. Receieved response: %s", rep)
+        return json.dumps(rep)
+
+
+    @Validator.isRequired(required=['Order_ID', 'Syom_Id', 'Status'])
+
+    def ExitBracketTrade(self, Order_Id, Syom_Id, Status) -> str :
+        """
+        Similar to Exit Cover order the functionality will ensure that any non executed open order will be cancelled. However for any orders which are executed it will automatically cancel one of the target or stop loss legs and modify the other leg to be placed as a market order. This will ensure that any executed orders will be squared off in position terms.
+
+       Exit Bracket Order
+
+       OrderId : Nest OrderId
+
+       Syom_Id : Syom_Id obtained post placing Bracket Order
+
+       Status: Current Status of the Bracket Order
+
+       """
+        LOGGER.info("ExitBracketTrade method is called.")
+        data = {'nstOrdNo': Order_Id, 'syomID': Syom_Id, 'sts': Status}
+        params = locals()
+        LOGGER.debug("ExitBracketTrade method is called with data: %s", data)
+        url = self.__router._ExitBracketTradeURL().format(userid=self.__constants.eqAccId)
+        resp = self.__http._DeleteMethod(url, json.dumps(data))
+        del (params["self"])
+        LOGGER.debug("Response receieved: %s", resp)
+        return json.dumps(resp)
+
+
+    @Validator.isRequired(required=['Exchange','Streaming_Symbol','Transaction_Type','Quantity','Duration','Limit_Price','Target','StopLoss','Trailing_Stop_Loss', 'Trailing_Stop_Loss_Value'])
+    @Validator.ValidateInputDataTypes
+
+    def PlaceBracketTrade(self, Exchange : ExchangeEnum, Streaming_Symbol, Transaction_Type : ActionEnum, Quantity : int, Duration : DurationEnum, Disclosed_Quantity, Limit_Price, Target, StopLoss, Trailing_Stop_Loss='Y', Trailing_Stop_Loss_Value="1") -> str or None:
+
+        """
+
+        Bracket Order
+
+        Exchange : Exchange
+
+        Transaction_Type : BUY/SELL
+
+        Duration : DAY/IOC/EOS(for BSE)
+
+        Order_Type: LIMIT/MARKET/STOP_LIMIT/STOP_MARKET
+
+        Quantity : Quantity of the scrip
+
+        Streaming_Symbol : companycode_exchange to be obtained from Contract file downloaded
+
+        Limit_Price : Limit price of scrip
+
+        Disclosed_Quantity : Quantity to be disclosed while order placement
+
+        Target : Absolute Target value
+
+        StopLoss :Absolute Stop Loss value
+
+        Trailing_Stop_Loss : Y/N
+
+        Trailing_Stop_Loss_Value : Number
+
+        """
+        LOGGER.info("PlaceBracketTrade method is called.")
+        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
+            print('Operation invalid for Commodities')
+            LOGGER.debug("Operation invalid for commodities.")
+            return
+
+        data = {'exc': Exchange, 'sym': Streaming_Symbol,
+                'trnsTyp': Transaction_Type, 'qty': Quantity, 'dur': Duration, 'dsQty': Disclosed_Quantity,
+                'prc': Limit_Price, 'trdBsdOn': "LTP", 'sqOffBsdOn': 'Absolute', 'sqOffVal': Target,
+                'slBsdOn': 'Absolute', 'slVal': StopLoss, 'trlSl': Trailing_Stop_Loss,
+                'trlSlVal': Trailing_Stop_Loss_Value, 'ordSrc': 'API'}
+        LOGGER.debug("PlaceBracketTrade method is called with data: %s", data)
+        url = self.__router._PlaceBracketTradeURL().format(userid=self.__constants.eqAccId)
+        resp = self.__http._PostMethod(url, json.dumps(data))
+        LOGGER.debug("Response received: %s", resp)
+        return json.dumps(resp)
+
+
+    def PlaceBasketTrade(self, orderlist : List[Order]) -> str :
+        """
+
+        Basket order allows user to place multiple orders at one time. User can place orders for multiple scrips all at once. One just creates multiple orders for same or different securities and club these orders together to be placed in one go. This helps save time.
+
+        orderlist : List of Order to be placed, Refer: Order Class
+
+        """
+        LOGGER.info("PlaceBasketTrade method is called.")
+        isComm = False
+        lst = []
+        for x in orderlist:
+            if x.exc == ExchangeEnum.MCX or x.exc == ExchangeEnum.NCDEX:
+                isComm = True
+                continue
+
+            #//FIXME: Find better implementation for validation in this method, current implimentation is redundant.
+            data = {'trdSym':   Validator.isRequiredv2('TradingSymbol', x.trdSym),
+                    'exc':      Validator.isRequiredv2('Exchange',x.exc),
+                    'action':   Validator.isRequiredv2('Action',x.action),
+                    'dur':      Validator.isRequiredv2('Duration',x.dur),
+                    'ordTyp':   Validator.isRequiredv2('OrderType',x.ordTyp),
+                    'qty':      Validator.isRequiredv2('Quantity',x.qty),
+                    'dscQty':   x.dscQty,
+                    'price':    Validator.isRequiredv2('Price',x.price),
+                    'trgPrc':   Validator.isRequiredv2('TriggerPrice',x.trgPrc),
+                    'prdCode':  Validator.product_code(Validator.isRequiredv2('ProductCode',x.prdCode), x.exc, self.__constants.ProductCodesMap),
+                    'vnCode': '',
+                    'rmk': ''}
+            lst.append(data)
+
+        fd = {
+            "ordLst": lst,
+            "ordSrc": "API"
+        }
+        if isComm == True:
+            print('Basket Order not available for Commodity')
+        LOGGER.debug("PlaceBasketTrade method is called with data: %s", fd)
+        url = self.__router._PlaceBasketTradeURL().format(userid=self.__constants.eqAccId)
+        resp = self.__http._PostMethod(url, json.dumps(fd))
+        LOGGER.debug("Response received: %s", resp)
+        return json.dumps(resp)
+
+
+    def Limits(self) -> str :
+        """
+        Limits refers to the cumulative margins available in your account which can be used for trading and investing in various products. Limits is a combination of the free cash you have (i.e. un-utilized cash), cash equivalent securities (usually margin pledged securities), any money which is in transit (T1/T2 day sell transaction values) and others, all of which can be used for placing orders. Usually whenever you place an order in a given asset and product type our risk management system assesses your limits available and then lets the orders go through or blocks the orders. Limits are dynamic in nature and can be influenced by the Mark to Markets in your positions and sometimes even by the LTP of your holdings.
+
+        Get limits
+
+
+        """
+        LOGGER.info("Limits method is called.")
+        LOGGER.debug("Limits method is called for accout type: %s",
+                self.__constants.Data['data']['lgnData']['accTyp'])
+        if self.__constants.Data['data']['lgnData']['accTyp'] == 'EQ':
+            url = self.__router._LimitsURL().format(userid=self.__constants.eqAccId)
+            resp = self.__http._GetMethod(url)
+            LOGGER.debug("Response recevied: %s", resp)
+            return json.dumps({"eq": resp, "comm": ""})
+
+        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'CO':
+            url = self.__router._LimitsURL_comm().format(userid=self.__constants.coAccId)
+            resp = self.__http._GetMethod(url)
+            LOGGER.debug("Response recevied: %s", resp)
+            return json.dumps({"eq": resp, "comm": resp})
+
+        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'COMEQ':
+            url = self.__router._LimitsURL().format(userid=self.__constants.eqAccId)
+            url_comm = self.__router._LimitsURL_comm().format(userid=self.__constants.coAccId)
+            rep = self.__http._GetMethod(url)
+            LOGGER.debug("Response recevied for eq: %s", rep)
+            rep_comm = self.__http._GetMethod(url_comm)
+            LOGGER.debug("Response recevied for comm: %s", rep_comm)
+            combine = {"eq": rep, "comm": rep_comm}
+            return json.dumps(combine)
+
+    @Validator.isRequired(required=['Exchange'])
+    @Validator.ValidateInputDataTypes
+
+    def GetAMOStatus(self, Exchange : ExchangeEnum = None) -> str :
+        """
+
+        Get AMO status of exchange
+
+        `Exchange` : Exchange to get AMO status of.
+
+        """
+        LOGGER.info("Limits method is called.")
+        LOGGER.debug("Limits method is called for accout type: %s",
+                self.__constants.Data['data']['lgnData']['accTyp'])
+
+        if self.__constants.Data['data']['lgnData']['accTyp'] == 'EQ':
+            url = self.__router._GetAMOFlag()
+            resp = self.__http._GetMethod(url)
+            LOGGER.debug("Response recevied: %s", resp)
+            return json.dumps({"eq": resp, "comm": ""})
+
+        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'CO':
+            url = self.__router._GetAMOFlag_comm().format(exch=Exchange)
+            resp = self.__http._GetMethod(url)
+            LOGGER.debug("Response recevied: %s", resp)
+            return json.dumps({"eq": "", "comm": resp})
+
+        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'COMEQ':
+            url = self.__router._GetAMOFlag()
+            url_comm = self.__router._GetAMOFlag_comm().format(exch=Exchange)
+            rep = self.__http._GetMethod(url)
+            LOGGER.debug("Response recevied for eq: %s", rep)
+            rep_comm = self.__http._GetMethod(url_comm)
+            LOGGER.debug("Response recevied for comm: %s", rep_comm)
+            combine = {"eq": rep, "comm": rep_comm}
+            return json.dumps(combine)
+
+
+    @Validator.isRequired(required=['Trading_Symbol','Exchange','Action','Duration','Order_Type','Quantity','Streaming_Symbol','Limit_Price','TriggerPrice', 'ProductCode'])
+    @Validator.ValidateInputDataTypes
+
+    def PlaceAMOTrade(self, Trading_Symbol, Exchange : ExchangeEnum, Action : ActionEnum, Duration : DurationEnum, Order_Type : OrderTypeEnum, Quantity : int, Streaming_Symbol, Limit_Price, Disclosed_Quantity="0", TriggerPrice="0", ProductCode : ProductCodeENum = ProductCodeENum.CNC) -> str :
+
+        """
+        After market order or AMO in short refers to orders which can be placed once the markets or exchanges are closed for trading. You can place AMO post market hours which will result in the order in question being placed automatically by 9:15 AM - 9:30 AM the next business day. AMO orders usually need to be limit orders in order to prevent inadvertent execution in case of adverse price movement in markets at beginning of day. AMO is a useful way to place your orders in case you do not have time to place orders during market hours.
+
+        After Market Order trade
+
+        Trading_Symbol : Trading Symbol of the Scrip
+
+        Exchange : Exchange
+
+        Action : BUY/SELL
+
+        Duration : DAY/IOC/EOS(for BSE)
+
+        Order_Type: LIMIT/MARKET/STOP_LIMIT/STOP_MARKET
+
+        Quantity : Quantity of the scrip
+
+        Streaming_Symbol : companycode_exchange to be obtained from Contract file downloaded
+
+        Limit_Price : Limit price of scrip
+
+        Disclosed_Quantity : Quantity to be disclosed while order placement
+
+        TriggerPrice : Trigger Price applicable for SL/SL-M Orders
+
+        ProductCode : CNC/MIS/NRML/MTF
+
+        """
+        LOGGER.info("PlaceAMOTrade method is called.")
+
+        data = {'trdSym': Trading_Symbol, 'exc': Exchange, 'action': Action, 'dur': Duration, 'flQty': "0",
+                'ordTyp': Order_Type, 'qty': Quantity, 'dscQty': Disclosed_Quantity, 'sym': Streaming_Symbol,
+                'mktPro': "",
+                'lmPrc': Limit_Price, 'trgPrc': TriggerPrice, 'prdCode': Validator.product_code(ProductCode.value, Exchange.value, self.__constants.ProductCodesMap), 'posSqr': "false",
+                'minQty': "0", 'ordSrc': "API", 'vnCode': '', 'rmk': ''}
+
+        LOGGER.debug("PlaceAMOTrade method is called with data: %s", data)
+        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
+            url = self.__router._PlaceAMOTrade_comm().format(userid=self.__constants.coAccId)
+            resp = self.__http._PostMethod(url, json.dumps(data))
+            LOGGER.debug("Response receieved: %s",resp)
+            return json.dumps(resp)
+
+        else:
+            url = self.__router._PlaceAMOTrade().format(userid=self.__constants.eqAccId)
+            resp = self.__http._PostMethod(url, json.dumps(data))
+            LOGGER.debug("Response receieved: %s",resp)
+            return json.dumps(resp)
+
+
+    @Validator.isRequired(required=['Trading_Symbol','Exchange','Action','Duration','Order_Type','Quantity','Streaming_Symbol','Limit_Price','Order_ID','TriggerPrice', 'ProductCode'])
+    @Validator.ValidateInputDataTypes
+
+    def ModifyAMOTrade(self, Trading_Symbol, Exchange : ExchangeEnum, Action : ActionEnum, Duration : DurationEnum, Order_Type : OrderTypeEnum, Quantity : int, Streaming_Symbol, Limit_Price, Order_ID, Disclosed_Quantity="0", TriggerPrice="0", ProductCode : ProductCodeENum = ProductCodeENum.CNC) -> str :
+
+        """
+
+        Modify After Market Order
+
+        Trading_Symbol : Trading Symbol of the Scrip
+
+        Exchange : Exchange
+
+        Action : BUY/SELL
+
+        Duration : DAY/IOC/EOS(for BSE)
+
+        Order_Type: LIMIT/MARKET/STOP_LIMIT/STOP_MARKET
+
+        Quantity : Quantity of the scrip
+
+        Streaming_Symbol : companycode_exchange to be obtained from Contract file downloaded
+
+        Limit_Price : Limit price of scrip
+
+        Disclosed_Quantity : Quantity to be disclosed while order placement
+
+        TriggerPrice : Trigger Price applicable for SL/SL-M Orders
+
+        ProductCode : CNC/MIS/NRML/MTF
+
+        """
+        LOGGER.info("ModifyAMOTrade method is called.")
+
+        data = {'trdSym': Trading_Symbol, 'exc': Exchange, 'action': Action, 'dur': Duration, 'flQty': "0",
+                'ordTyp': Order_Type, 'qty': Quantity, 'dscQty': Disclosed_Quantity, 'sym': Streaming_Symbol,
+                'mktPro': "",
+                'lmPrc': Limit_Price, 'trgPrc': TriggerPrice, 'prdCode': Validator.product_code(ProductCode.value, Exchange.value, self.__constants.ProductCodesMap), 'dtDays': '', 'nstOID': Order_ID}
+        LOGGER.debug("ModifyAMOTrade method is called with data: %s", data)
+
+        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
+            url = self.__router._ModifyAMOTrade_comm().format(userid=self.__constants.coAccId)
+            resp = self.__http._PutMethod(url, json.dumps(data))
+            LOGGER.debug("Response receieved: %s",resp)
+            return json.dumps(resp)
+
+        else:
+            url = self.__router._ModifyAMOTrade().format(userid=self.__constants.eqAccId)
+            resp = self.__http._PutMethod(url, json.dumps(data))
+            LOGGER.debug("Response receieved: %s",resp)
+            return json.dumps(resp)
+
+
+    @Validator.isRequired(required=['Order_ID','Exchange','Order_Type','ProductCode'])
+    @Validator.ValidateInputDataTypes
+
+    def CancelAMOTrade(self, Order_ID, Exchange : ExchangeEnum, Order_Type : OrderTypeEnum, ProductCode : ProductCodeENum) -> str :
+        """
+
+        Cancel After Market Order
+
+        OrderId : Nest Order Id
+
+        """
+        LOGGER.info("CancelAMOTrade method is called.")
+        data = {"nstOID": Order_ID, "exc": Exchange, "prdCode": Validator.product_code(ProductCode.value, Exchange.value, self.__constants.ProductCodesMap), "ordTyp": Order_Type}
+        LOGGER.debug("CancelAMOTrade method is called with data: %s", data)
+        if Exchange == ExchangeEnum.MCX or Exchange == ExchangeEnum.NCDEX:
+            url = self.__router._CancelAMOTrade_comm().format(userid=self.__constants.coAccId)
+            resp = self.__http._PutMethod(url, json.dumps(data))
+            LOGGER.debug("Response received: %s", resp)
+            return json.dumps(resp)
+
+        else:
+            url = self.__router._CancelAMOTrade().format(userid=self.__constants.eqAccId)
+            resp = self.__http._PutMethod(url, json.dumps(data))
+            LOGGER.debug("Response received: %s", resp)
+            return json.dumps(resp)
+
+
+    def PositionSquareOff(self, orderlist : List[Order]) -> str :
+        """
+
+        Square off is a term used in intraday and simply means closing all open positions by the end of the trading day
+
+        orderList : List of orders to be Squared Off. Refer : Orders class.
+
+        """
+        lst_eq = []
+        lst_comm = []
+        LOGGER.info("PositionSquareOff method is called.")
+        for x in orderlist:
+
+            if x.exc == ExchangeEnum.MCX or x.exc == "NCDEX":
+            #//FIXME: Find better implementation for validation in this method, current implimentation is redundant.
+                data = {'trdSym':   Validator.isRequiredv2('TradingSymbol', x.trdSym),
+                        'exc':      Validator.isRequiredv2('Exchange', x.exc),
+                        'action':   Validator.isRequiredv2('Action', x.action),
+                        'dur':      Validator.isRequiredv2('Duration', x.dur),
+                        'flQty':    "0",
+                        'ordTyp':   Validator.isRequiredv2('OrderType',x.ordTyp),
+                        'qty':      Validator.isRequiredv2('Quantity', x.qty),
+                        'dscQty':   x.dscQty,
+                        'sym':      Validator.isRequiredv2('StreamingSymbol',x.sym),
+                        'mktPro':   "",
+                        'lmPrc':    Validator.isRequiredv2('Price', x.price),
+                        'trgPrc':   Validator.isRequiredv2('TriggerPrice', x.trgPrc),
+                        'prdCode':  Validator.product_code(Validator.isRequiredv2('ProductCode',x.prdCode), x.exc, self.__constants.ProductCodesMap),
+                        'dtDays':   '',
+                        'posSqr':   "true",
+                        'minQty':   "0",
+                        'ordSrc':   "API",
+                        'vnCode':   '',
+                        'rmk':      ''}
+                lst_comm.append(data)
+            else:
+                data = {'trdSym':   Validator.isRequiredv2('TradingSymbol', x.trdSym),
+                        'exc':      Validator.isRequiredv2('Exchange', x.exc),
+                        'action':   Validator.isRequiredv2('Action', x.action),
+                        'dur':      Validator.isRequiredv2('Duration', x.dur),
+                        'flQty':    "0",
+                        'ordTyp':   Validator.isRequiredv2('OrderType',x.ordTyp),
+                        'qty':      Validator.isRequiredv2('Quantity', x.qty),
+                        'dscQty':   x.dscQty,
+                        'sym':      Validator.isRequiredv2('StreamingSymbol',x.sym),
+                        'mktPro':   "",
+                        'lmPrc':    Validator.isRequiredv2('Price', x.price),
+                        'trgPrc':   Validator.isRequiredv2('TriggerPrice', x.trgPrc),
+                        'prdCode':  Validator.product_code(Validator.isRequiredv2('ProductCode',x.prdCode), x.exc, self.__constants.ProductCodesMap),
+                        'dtDays':   '',
+                        'posSqr':   "true",
+                        'minQty':   "0",
+                        'ordSrc':   "API",
+                        'vnCode':   '',
+                        'rmk':      ''}
+                lst_eq.append(data)
+
+        resp_eq = ""
+        resp_comm = ""
+
+        if len(lst_eq) > 0:
+            url = self.__router._PositionSqOffURL().format(userid=self.__constants.eqAccId)
+            LOGGER.debug("PositionSquareOff method is called with data: %s.", lst_eq)
+            resp_eq = self.__http._PostMethod(url, json.dumps(lst_eq))
+
+        if len(lst_comm) > 0:
+            url_comm = self.__router._PositionSqOffURL().format(userid=self.__constants.coAccId)
+            LOGGER.debug("PositionSquareOff method is called with data: %s.", lst_comm)
+            resp_comm = self.__http._PostMethod(url_comm, json.dumps(lst_comm))
+
+        resp = {"eq": resp_eq, "comm": resp_comm}
+        LOGGER.debug("Response received: %s", resp)
+        return json.dumps(resp)
+
+
+    @Validator.isRequired(required=['Streaming_Symbol','Conversion_Type', 'Quantity', 'Action', 'Old_Product_Code', 'New_Product_Code','Exchange','Trading_Symbol'])
+    @Validator.ValidateInputDataTypes
+
+    def ConvertPositionCOMM(self, Streaming_Symbol, Conversion_Type, Quantity, Action : ActionEnum, Old_Product_Code : ProductCodeENum, New_Product_Code : ProductCodeENum, Exchange : ExchangeEnum, Trading_Symbol) -> str :
+        """
+        Convert a Position partially
+
+        `Streaming_Symbol` : companycode_exchange to be obtained from Contract file downloaded
+
+        `Conversion_Type` : 'D' - Daywise and 'C' - Carry forward position
+
+        `Quantity` : Quantity to be converted
+
+        `Action` : BUY/SELL
+
+        `Old_Product_Code` : Existing Product Code of the trade
+
+        `New_Product_Code`: New Product code of the trade
+
+        `Exchange` : Exchange
+
+        `Trading_Symbol` : Trading Symbol of the Scrip
+
+        """
+        LOGGER.info("ConvertPositionCOMM method is called.")
+
+        data = {
+            "sym": Streaming_Symbol,
+            "cnvTyp": Conversion_Type,
+            "qty": Quantity,
+            "action": ApiUtils.getAlternateActionName(Action.BUY),
+            "prdCode": Validator.product_code(Old_Product_Code.value, Exchange.value, self.__constants.ProductCodesMap),
+            "prdCodeCh": Validator.product_code(New_Product_Code.value, Exchange.value, self.__constants.ProductCodesMap),
+            "ordSrc": "API",
+            "exc": Exchange,
+            "trdSym": Trading_Symbol
+        }
+
+        LOGGER.debug("ConvertPositionCOMM method is called with data %s",data)
+        url = self.__router._ConvertPositionURL_comm().format(userid=self.__constants.coAccId)
+        resp = self.__http._PutMethod(url, json.dumps(data))
+        LOGGER.debug("Response receieved: %s", resp)
+        return json.dumps(resp)
+
+    @Validator.isRequired(required=['Order_ID','Fill_Id','New_Product_Code','Old_Product_Code','Exchange','Order_Type'])
+    @Validator.ValidateInputDataTypes
+
+    def ConvertPosition(self, Order_ID, Fill_Id, New_Product_Code : ProductCodeENum, Old_Product_Code : ProductCodeENum, Exchange : ExchangeEnum, Order_Type : OrderTypeEnum) -> str :
+        """
+
+        Convert Position : converts your holding position from MIS to CNC and vice-versa
+
+        `Order_ID` : Nest Order id
+
+        `Fill_Id` : Fill Id of the trade obtained from Trade API
+
+        `New_Product_Code` : New Product code of the trade
+
+        `Old_Product_Code` : Existing Product Code of the trade
+
+        `Exchange` : Exchange
+
+        `Order_Type`: LIMIT/MARKET/STOP_LIMIT/STOP_MARKET
+
+        """
+        LOGGER.info("ConvertPosition method is called.")
+        data = {'nstOID': Order_ID, 'flID': Fill_Id,
+                'prdCodeCh': New_Product_Code, 'prdCode': Old_Product_Code,
+                'exc': Exchange, 'ordTyp': Order_Type}
+
+        LOGGER.debug("ConvertPosition method is called with data %s",data)
+        url = self.__router._ConvertPositionURL().format(userid=self.__constants.eqAccId)
+        resp = self.__http._PutMethod(url, json.dumps(data))
+        LOGGER.debug("Response receieved: %s", resp)
+        return json.dumps(resp)
+
+
+    # MF Methods
+
+
+    @Validator.ValidateInputDataTypes
+
+    def PlaceMF(self, Token, ISIN_Code, Transaction_Type, Client_Code, Quantity, Amount, ReInv_Flag, Folio_Number, Scheme_Name, Start_Date, End_Date, SIP_Frequency, Generate_First_Order_Today, Scheme_Plan, Scheme_Code, Mandate_Id) -> str :
+
+        '''
+
+        Token:
+
+        ISIN_Code:
+
+        Transaction_Type:
+
+        Client_Code:
+
+        Quantity:
+
+        Amount:
+
+        ReInv_Flag:
+
+        Folio_Number:
+
+        Order_Type:
+
+        Scheme_Name:
+
+        Start_Date:
+
+        End_Date:
+
+        SIP_Frequency:
+
+        Generate_First_Order_Today:
+
+        Scheme_Plan:
+
+        Scheme_Code:
+
+
+        '''
+        LOGGER.info("PlaceMF method is called.")
+        data = {'currentOrdSts': '', 'token': Token, 'isin': ISIN_Code, 'txnTyp': Transaction_Type,
+                'clientCode': Client_Code, 'qty': Quantity, 'amt': Amount, 'reInvFlg': ReInv_Flag,
+                'reqstdBy': self.__constants.eqAccId, 'folioNo': Folio_Number,
+                'ordTyp': 'FRESH', 'txnId': '0', 'schemeName': Scheme_Name, 'rmrk': '',
+                'mnRdmFlg': '', 'ordSrc': 'API', 'strtDy': "1", 'strtDt': Start_Date, 'endDt': End_Date,
+                'sipFrq': SIP_Frequency, 'gfot': Generate_First_Order_Today, 'tnr': '999',
+                'mdtId': Mandate_Id, 'sipregno': '', 'siporderno': '',
+                'schemePlan': Scheme_Plan, 'schemeCode': Scheme_Code, 'euinnumber': '', 'dpc': 'Y',
+                'closeAccountFlag': 'N',
+                'kycflag': '1', 'euinflag': 'N', 'physicalFlag': 'D'}
+
+        LOGGER.info("PlaceMF method is called with data: %s.", data)
+        url = self.__router._PlaceMFURL().format(userid=self.__constants.eqAccId)
+        resp = self.__http._PostMethod(url, json.dumps(data))
+        LOGGER.debug("Response received: %s", resp )
+        return json.dumps(resp)
+
+
+    @Validator.ValidateInputDataTypes
+
+    def ModifyMF(self, Token, ISIN_Code, Transaction_Type, Client_Code, Quantity, Amount, ReInv_Flag, Folio_Number, Scheme_Name, Start_Date, End_Date, SIP_Frequency, Generate_First_Order_Today, Scheme_Plan, Scheme_Code, Transaction_Id, Mandate_Id) -> str :
+
+        '''
+
+        certain attributes of a MF order may be modified., as long as on order is open or pending in the system
+
+        Token:
+
+        ISIN_Code:
+
+        Transaction_Type:
+
+        Client_Code:
+
+        Quantity:
+
+        Amount:
+
+        ReInv_Flag:
+
+        Folio_Number:
+
+        Order_Type:
+
+        Scheme_Name:
+
+        Start_Date:
+
+        End_Date:
+
+        SIP_Frequency:
+
+        Generate_First_Order_Today:
+
+        Scheme_Plan:
+
+        Scheme_Code:
+
+
+        '''
+        LOGGER.info("ModifyMF method is called.")
+        data = {'currentOrdSts': 'ACCEPTED', 'token': Token, 'isin': ISIN_Code, 'txnTyp': Transaction_Type,
+                'clientCode': Client_Code, 'qty': Quantity, 'amt': Amount, 'reInvFlg': ReInv_Flag,
+                'reqstdBy': self.__constants.eqAccId, 'folioNo': Folio_Number,
+                'ordTyp': 'MODIFY', 'txnId': Transaction_Id, 'schemeName': Scheme_Name, 'rmrk': '',
+                'mnRdmFlg': '', 'ordSrc': 'API', 'strtDy': "1", 'strtDt': Start_Date, 'endDt': End_Date,
+                'sipFrq': SIP_Frequency, 'gfot': Generate_First_Order_Today, 'tnr': '999',
+                'mdtId': Mandate_Id, 'sipregno': '', 'siporderno': '',
+                'schemePlan': Scheme_Plan, 'schemeCode': Scheme_Code, 'euinnumber': '', 'dpc': 'Y',
+                'closeAccountFlag': 'N',
+                'kycflag': '1', 'euinflag': 'N', 'physicalFlag': 'D'}
+
+        LOGGER.debug("PlaceMF method is called with data: %s.", data)
+        url = self.__router._PlaceMFURL().format(userid=self.__constants.eqAccId)
+        resp = self.__http._PutMethod(url, json.dumps(data))
+        LOGGER.debug("Response received: %s", resp )
+        return json.dumps(resp)
+
+
+    @Validator.ValidateInputDataTypes
+
+    def CancelMF(self, Token, ISIN_Code, Transaction_Type, Client_Code, Quantity, Amount, ReInv_Flag, Folio_Number, Scheme_Name, Start_Date, End_Date, SIP_Frequency, Generate_First_Order_Today, Scheme_Plan, Scheme_Code, Transaction_Id) -> str :
+
+        '''
+
+        Token:
+
+        ISIN_Code:
+
+        Transaction_Type:
+
+        Client_Code:
+
+        Quantity:
+
+        Amount:
+
+        ReInv_Flag:
+
+        Folio_Number:
+
+        Scheme_Name:
+
+        Start_Date:
+
+        End_Date:
+
+        SIP_Frequency:
+
+        Generate_First_Order_Today:
+
+        Scheme_Plan:
+
+        Scheme_Code:
+
+        '''
+        LOGGER.info("CancelMF method is called.")
+        data = {'currentOrdSts': 'ACCEPTED', 'token': Token, 'isin': ISIN_Code, 'txnTyp': Transaction_Type,
+                'clientCode': Client_Code, 'qty': Quantity, 'amt': Amount, 'reInvFlg': ReInv_Flag,
+                'reqstdBy': self.__constants.eqAccId, 'folioNo': Folio_Number,
+                'ordTyp': 'CANCEL', 'txnId': Transaction_Id, 'schemeName': Scheme_Name, 'rmrk': '',
+                'mnRdmFlg': '', 'ordSrc': 'API', 'strtDy': "1", 'strtDt': Start_Date, 'endDt': End_Date,
+                'sipFrq': SIP_Frequency, 'gfot': Generate_First_Order_Today, 'tnr': '999',
+                'mdtId': '', 'sipregno': '', 'siporderno': '',
+                'schemePlan': Scheme_Plan, 'schemeCode': Scheme_Code, 'euinnumber': '', 'dpc': 'Y',
+                'closeAccountFlag': 'N',
+                'kycflag': '1', 'euinflag': 'N', 'physicalFlag': 'D'}
+
+        LOGGER.debug("CancelMF with data %s", data)
+        url = self.__router._CancelMFURL().format(userid=self.__constants.eqAccId)
+        resp = self.__http._PutMethod(url, json.dumps(data))
+        LOGGER.debug("Response recevied: %s", resp)
+        return json.dumps(resp)
+
+
+    def HoldingsMF(self) -> str :
+        LOGGER.info("HoldingsMF method is called.")
+        params = locals()
+        del (params["self"])
+        url = self.__router._HoldingsMFURL().format(userid=self.__constants.eqAccId)
+        resp = self.__http._GetMethod(url)
+        LOGGER.info("HoldingsMF method is called. Response recevied: %s",resp)
+        return json.dumps(resp)
+
+    # Chart methods
+
+    def __getChartDataOfScrip(self, Exchange, AssetType, Streaming_Symbol, Interval, TillDate = None, IncludeContinuousFutures = False) -> str :
+
+        LOGGER.info("Inside __getChartDataOfScrip method.")
+
+        # If asset type is not amongst "FUTCOM", "FUTCUR", "FUTSTK", "FUTIDX", set IncludeContinuousFutures as FALSE
+        if AssetType not in [AssetTypeEnum.FUTCOM, AssetTypeEnum.FUTCUR, AssetTypeEnum.FUTIDX, AssetTypeEnum.FUTIDX]:
+            IncludeContinuousFutures = False
+
+        data = {'chTyp' : "Interval",
+                'conti' : IncludeContinuousFutures,
+                'ltt' : TillDate
+                }
+
+        LOGGER.debug("__getChartDataOfScrip method is called with data: %s", data)
+
+        url = self.__router._ChartsURL().format(interval = Interval, exc = Exchange, aTyp = AssetType, symbol = Streaming_Symbol)
+        reply = self.__http._PostMethod(url, json.dumps(data))
+
+        if reply != "":
+            reply = ChartResponseFormatter(reply).getOHCLResponse()
+            LOGGER.debug("Response received: %s", reply)
+        return json.dumps(reply)
+
+
+    @Validator.isRequired(required=['Exchange', 'AssetType', 'Interval', 'Streaming_Symbol'])
+    @Validator.ValidateInputDataTypes
+
+    def getIntradayChart(self, Exchange : ChartExchangeEnum, AssetType : AssetTypeEnum, Streaming_Symbol, Interval : IntradayIntervalEnum, TillDate = None, IncludeContinuousFutures : bool = False) -> str :
+        """
+        - `Exchange` : Exchange
+        - `AssetType` : AssetType for the chart
+        - `Streaming_Symbol` : Symbol to fetch chart data for. Eg: 11536_NSE, 4963_BSE, -29 etc
+        - `Interval` : interval for Intraday charts
+        - `TillDate` : Charts data to fetch till date (format : yyyy-MM-dd)
+        - `IncludeContinuousFutures` : boolean. True -> If Continous Futures required. Valid only for instruments (Asset Types) - FUTIDX,FUTSTk,FUTCUR,FUTCOM
+        """
+
+        LOGGER.info("getIntradayChart method is called.")
+
+        response = self.__getChartDataOfScrip(Exchange, AssetType, Streaming_Symbol, Interval, TillDate, IncludeContinuousFutures)
+
+        return response
+
+    @Validator.isRequired(required=['Exchange', 'AssetType', 'Interval', 'Streaming_Symbol'])
+    @Validator.ValidateInputDataTypes
+
+    def getEODChart(self, Exchange : ChartExchangeEnum, AssetType : AssetTypeEnum, Streaming_Symbol, Interval : EODIntervalEnum, TillDate = None, IncludeContinuousFutures : bool = False) -> str :
+        """
+        - `Exchange` : Exchange
+        - `AssetType` : AssetType for the chart
+        - `Streaming_Symbol` : Symbol to fetch chart data for. Eg: 11536_NSE, 4963_BSE, -29 etc
+        - `Interval` : interval for EOD charts
+        - `TillDate` : Charts data to fetch till date (format : yyyy-MM-dd)
+        - `IncludeContinuousFutures` : boolean. True -> If Continous Futures required. Valid only for instruments (Asset Types) - FUTIDX,FUTSTk,FUTCUR,FUTCOM
+        """
+
+        LOGGER.info("getEODChart method is called.")
+
+        response = self.__getChartDataOfScrip(Exchange, AssetType, Streaming_Symbol, Interval, TillDate, IncludeContinuousFutures)
+
+        return response
+
+
+    # Live News methods
+
+    def getNewsCategories(self) -> str:
+        LOGGER.info("getNewsCategories method is called")
+        service = LiveNewsService(self.__router, self.__http, self.__constants.Filename)
+        try:
+            response = service._getNewsCategories()
+        except OSError as e:
+            raise e
+        LOGGER.debug(f"getNewsCategories response is : {response}")
+        return response
+
+    @Validator.ValidateInputDataTypes
+    def getLiveNews(self, holdings : bool, category : str = None, searchText : str = None, pageNumber : int = None) -> str :
+        LOGGER.info("getLiveNews method is called")
+
+        service = LiveNewsService(self.__router, self.__http, self.__constants.Filename)
+        try:
+            if holdings:
+                response = service._getHoldingsNews(category, searchText, pageNumber)
+            else:
+                response = service._getGeneralNews(category, searchText, pageNumber)
+        except OSError as e:
+            raise e
+
+        LOGGER.debug(f"getLiveNews response is : {response}")
+        return response
+
+    @Validator.ValidateInputDataTypes
+    def getNewsForResultsAndStocks(self, holdings : bool, searchText : str = None, pageNumber : int = None) -> str :
+        LOGGER.info("getNewsForResultsAndStocks method is called")
+
+
+        service = LiveNewsService(self.__router, self.__http, self.__constants.Filename)
+        try:
+            if holdings:
+                response = service._getHoldingsNews(["Results", "Stocks in News"], searchText, pageNumber)
+            else:
+                response = service._getResultsAndStocksNews(searchText, pageNumber)
+        except OSError as e:
+            raise e
+
+        LOGGER.debug(f"getNewsForResultsAndStocks response is : {response}")
+        return response
+
+    @Validator.isRequired(['symbol'])
+    @Validator.ValidateInputDataTypes
+    def getLatestCorporateActions(self, symbol : str) :
+        LOGGER.info("getLatestCorporateActions method is called")
+
+        service = LiveNewsService(self.__router, self.__http, self.__constants.Filename)
+        response = service._getLatestCorpActionsAPI(symbol)
+
+        LOGGER.debug(f"getLatestCorporateActions response is : {response}")
+        return response
+
+    # Streaming methods
+
+    def initQuotesStreaming(self) :
+        return QuotesFeed(self.__feedObj)
+
+    def initOrdersStreaming(self, acc_id : str, user_id : str) :
+        return OrdersFeed(self.__feedObj, acc_id, user_id)
+
+    def initLiveNewsStreaming(self) :
+        return LiveNewsFeed(self.__feedObj)
+
+    # Watchlist methods
+
+    def getWatchlistGroups(self):
+        LOGGER.info("getWatchlistGroups method is called.")
+        service = WatchlistService(self.__router, self.__http, self.__constants)
+
+        response = service._getWatchlistGroups()
+
+        LOGGER.debug(f'getWatchlistGroups response is : {response}')
+        return response
+
+    @Validator.isRequired(['GroupName'])
+    @Validator.ValidateInputDataTypes
+
+    def getWatchlistScrips(self, GroupName : str):
+        LOGGER.info("getWatchlistScrips method is called.")
+        service = WatchlistService(self.__router, self.__http, self.__constants)
+
+        response = service._getScripsOfGroup(GroupName)
+
+        LOGGER.debug(f'getWatchlistScrips response is : {response}')
+        return response
+
+    @Validator.isRequired(['GroupName', 'Symbols'])
+    @Validator.ValidateInputDataTypes
+
+    def createWatchlistGroup(self, GroupName : str, Symbols : list):
+        LOGGER.info("createWatchlistGroup method is called.")
+        service = WatchlistService(self.__router, self.__http, self.__constants)
+
+        response = service._createGroup(GroupName, Symbols)
+
+        LOGGER.debug(f'createWatchlistGroup response is : {response}')
+        return response
+
+    @Validator.isRequired(['GroupName', 'Symbols'])
+    @Validator.ValidateInputDataTypes
+    def addSymbolsWatchlist(self, GroupName : str, Symbols : list):
+        LOGGER.info("addSymbolsWatchlist method is called.")
+        service = WatchlistService(self.__router, self.__http, self.__constants)
+
+        response = service._addSymbols(GroupName, Symbols)
+
+        LOGGER.debug(f'addSymbolsWatchlist response is : {response}')
+        return response
+
+    @Validator.isRequired(['GroupName', 'Symbols'])
+    @Validator.ValidateInputDataTypes
+    def deleteSymbolsWatchlist(self, GroupName : str, Symbols : list):
+        LOGGER.info("deleteSymbolsWatchlist method is called.")
+        service = WatchlistService(self.__router, self.__http, self.__constants)
+
+        response = service._deleteSymbols(GroupName, Symbols)
+
+        LOGGER.debug(f'deleteSymbolsWatchlist response is : {response}')
+        return response
+
+    @Validator.isRequired(['GroupNames'])
+    @Validator.ValidateInputDataTypes
+    def deleteWatchlistGroups(self, GroupNames : list):
+        LOGGER.info("deleteWatchlistGroups method is called.")
+        service = WatchlistService(self.__router, self.__http, self.__constants)
+
+        response = service._deleteGroups(GroupNames)
+
+        LOGGER.debug(f'deleteWatchlistGroups response is : {response}')
+        return response
+
+    @Validator.isRequired(['GroupName', 'NewGroupName'])
+    @Validator.ValidateInputDataTypes
+    def renameWatchlistGroup(self, GroupName : str, NewGroupName : str):
+        LOGGER.info("renameWatchlistGroup method is called.")
+        service = WatchlistService(self.__router, self.__http, self.__constants)
+
+        response = service._renameGroup(GroupName, NewGroupName)
+
+        LOGGER.debug(f'renameWatchlistGroup response is : {response}')
+        return response
+
+
+    # Login methods
+
+    def Logout(self) -> None:
+        LOGGER.info("Logout method called.")
+        LOGGER.debug("Logout method called with account type: %s",
+            self.__constants.Data['data']['lgnData']['accTyp'])
+        params = locals()
+        del (params["self"])
+        if self.__constants.Data['data']['lgnData']['accTyp'] == 'EQ':
+            url = self.__router._LogoutURL().format(userid=self.__constants.eqAccId)
+            rep = self.__http._PutMethod(url, {})
+
+        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'CO':
+            url = self.__router._LogoutURL().format(userid=self.__constants.coAccId)
+            rep = self.__http._PutMethod(url, {})
+
+        elif self.__constants.Data['data']['lgnData']['accTyp'] == 'COMEQ':
+            url = self.__router._LogoutURL().format(userid=self.__constants.eqAccId)
+            rep = self.__http._PutMethod(url, {})
+
+        if rep != "":
+            if path.exists(self.__filename):
+                LOGGER.debug("File with account related details is removed.")
+                os.remove(self.__filename)
             self.__constants.Data = ""
```

### Comparing `APIConnect-2.0.1.post1/APIConnect/http.py` & `APIConnect-2.0.2/APIConnect/http.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-import json
-import logging
-from os import path
-import os
-import sys
-import requests
-
-ModuleLOGGER = logging.getLogger(__name__)
-
-def init_proxies(conf):
-    """
-    Method to load proxy parameters from configuration file.
-    - Parameter:
-        conf: ConfigParser object of provided configuration file.
-    """
-
-    if conf and 'PROXY' in conf:
-        if conf['PROXY'].get('HTTPS_PROXY') and conf['PROXY'].get('HTTP_PROXY'):
-            ModuleLOGGER.info("Found proxy related configurations.")
-            return {
-                    'http': conf['PROXY'].get('HTTP_PROXY'),
-                    'https': conf['PROXY'].get('HTTPS_PROXY'),
-                }
-    return {}
-
-class Http:
-    def __init__(self, constants, proxies, ssl_verify=False):
-
-        self.LOGGER = logging.getLogger(__name__)
-        self.LOGGER.info("Http object is being created.")
-
-        self.__constants = constants
-        self.__requests = requests.session()
-        if proxies:
-            self.LOGGER.debug("Proxies are setup for HTTP requests.")
-            self.__requests.proxies.update(proxies)
-            self.__requests.verify = ssl_verify
-
-    def _GetMethod(self, url : str, queryParams : dict = None, sendSource=True):
-        if sendSource:
-            self.LOGGER.debug("Request to url: %s", url)
-            response = self.__requests.get(url, headers={
-                "Authorization": self.__constants.JSessionId,
-                "Source": self.__constants.ApiKey,
-                "SourceToken": self.__constants.VendorSession,
-                "AppIdKey": self.__constants.AppIdKey
-                },
-                params=queryParams)
-        else:
-            self.LOGGER.debug("Request to url: %s", url)
-            response = self.__requests.get(url, headers={
-                "Authorization": self.__constants.JSessionId,
-                "SourceToken": self.__constants.VendorSession,
-                "AppIdKey": self.__constants.AppIdKey
-                },
-                params=queryParams)
-        if response.headers.get('AppIdKey') != "":
-            self.__constants.AppIdKey = response.headers.get('AppIdKey')
-
-        if response.status_code == 200:
-            return json.loads(response.content)
-        elif 200 < response.status_code <= 299:
-            self.LOGGER.debug("Response received with status code != 200.")
-            self.LOGGER.debug("Error response: %s", response.content.decode('UTF-8'))
-            return ""
-        else:
-            if 'Expired' in response.content.decode('UTF-8'):
-                print(json.dumps(json.loads(response.content.decode('UTF-8'))))
-                if path.exists(self.__constants.Filename):
-                    os.remove(self.__constants.Filename)
-                    sys.exit()
-                print("Expired session.")
-            print(response.content.decode('UTF-8'))
-            self.LOGGER.debug("Error response: %s", response.content.decode('UTF-8'))
-            return ""
-
-    def _PostMethod(self, url : str, data : str, sendSource=True):
-        if sendSource:
-            response = self.__requests.post(url, headers={
-                "Authorization": self.__constants.JSessionId,
-                "Source": self.__constants.ApiKey,
-                "SourceToken": self.__constants.VendorSession,
-                "AppIdKey": self.__constants.AppIdKey,
-                "Content-type": "application/json"}, data=data)
-
-        else:
-            response = self.__requests.post(url, headers={
-                "Authorization": self.__constants.JSessionId,
-                "SourceToken": self.__constants.VendorSession,
-                "AppIdKey": self.__constants.AppIdKey,
-                "Content-type": "application/json"}, data=data)
-
-        if response.headers.get('AppIdKey') != "":
-            self.__constants.AppIdKey = response.headers.get('AppIdKey')
-        if response.status_code == 200:
-            return json.loads(response.content)
-        else:
-            if 'Expired' in response.content.decode('UTF-8'):
-                print(json.dumps(json.loads(response.content.decode('UTF-8'))))
-                if path.exists(self.__constants.Filename):
-                    os.remove(self.__constants.Filename)
-                print("Expired session.")
-            self.LOGGER.debug("Error response: %s", response.content.decode('UTF-8'))
-            return ""
-
-    def _PutMethod(self, url : str, data : str):
-        response = self.__requests.put(url, headers={"Authorization": self.__constants.JSessionId,
-                                                "Source": self.__constants.ApiKey,
-                                                "SourceToken": self.__constants.VendorSession,
-                                                "AppIdKey": self.__constants.AppIdKey,
-                                                "Content-type": "application/json"}, data=data)
-        if response.headers.get('AppIdKey') != "":
-            self.__constants.AppIdKey = response.headers.get('AppIdKey')
-        if response.status_code == 200:
-            return json.loads(response.content)
-
-        else:
-            if 'Expired' in response.content.decode('UTF-8'):
-                if path.exists(self.__constants.Filename):
-                    os.remove(self.__constants.Filename)
-                print("Expired session.")
-            self.LOGGER.debug("Error response: %s", response.content.decode('UTF-8'))
-            return ""
-
-    def _DeleteMethod(self, url : str, data : str):
-        response = self.__requests.delete(url, headers={"Authorization": self.__constants.JSessionId,
-                                                    "Source": self.__constants.ApiKey,
-                                                    "SourceToken": self.__constants.VendorSession,
-                                                    "AppIdKey": self.__constants.AppIdKey,
-                                                    "Content-type": "application/json"}, data=data)
-        if response.headers.get('AppIdKey') != "":
-            self.__constants.AppIdKey = response.headers.get('AppIdKey')
-        if response.status_code == 200:
-            return json.loads(response.content)
-
-        else:
-            if 'Expired' in response.content.decode('UTF-8'):
-                if path.exists(self.__constants.Filename):
-                    os.remove(self.__constants.Filename)
-                print("Expired session.")
-            self.LOGGER.debug("Error response: %s", response.content.decode('UTF-8'))
-            return ""
-
-
+import json
+import logging
+from os import path
+import os
+import sys
+import requests
+
+ModuleLOGGER = logging.getLogger(__name__)
+
+def init_proxies(conf):
+    """
+    Method to load proxy parameters from configuration file.
+    - Parameter:
+        conf: ConfigParser object of provided configuration file.
+    """
+
+    if conf and 'PROXY' in conf:
+        if conf['PROXY'].get('HTTPS_PROXY') and conf['PROXY'].get('HTTP_PROXY'):
+            ModuleLOGGER.info("Found proxy related configurations.")
+            return {
+                    'http': conf['PROXY'].get('HTTP_PROXY'),
+                    'https': conf['PROXY'].get('HTTPS_PROXY'),
+                }
+    return {}
+
+class Http:
+    def __init__(self, constants, proxies, ssl_verify=False):
+
+        self.LOGGER = logging.getLogger(__name__)
+        self.LOGGER.info("Http object is being created.")
+
+        self.__constants = constants
+        self.__requests = requests.session()
+        if proxies:
+            self.LOGGER.debug("Proxies are setup for HTTP requests.")
+            self.__requests.proxies.update(proxies)
+            self.__requests.verify = ssl_verify
+
+    def _GetMethod(self, url : str, queryParams : dict = None, sendSource=True):
+        if sendSource:
+            self.LOGGER.debug("Request to url: %s", url)
+            response = self.__requests.get(url, headers={
+                "Authorization": self.__constants.JSessionId,
+                "Source": self.__constants.ApiKey,
+                "SourceToken": self.__constants.VendorSession,
+                "AppIdKey": self.__constants.AppIdKey
+                },
+                params=queryParams)
+        else:
+            self.LOGGER.debug("Request to url: %s", url)
+            response = self.__requests.get(url, headers={
+                "Authorization": self.__constants.JSessionId,
+                "SourceToken": self.__constants.VendorSession,
+                "AppIdKey": self.__constants.AppIdKey
+                },
+                params=queryParams)
+        if response.headers.get('AppIdKey') != "":
+            self.__constants.AppIdKey = response.headers.get('AppIdKey')
+
+        if response.status_code == 200:
+            return json.loads(response.content)
+        elif 200 < response.status_code <= 299:
+            self.LOGGER.debug("Response received with status code != 200.")
+            self.LOGGER.debug("Error response: %s", response.content.decode('UTF-8'))
+            return ""
+        else:
+            if 'Expired' in response.content.decode('UTF-8'):
+                print(json.dumps(json.loads(response.content.decode('UTF-8'))))
+                if path.exists(self.__constants.Filename):
+                    os.remove(self.__constants.Filename)
+                    sys.exit()
+                print("Expired session.")
+            print(response.content.decode('UTF-8'))
+            self.LOGGER.debug("Error response: %s", response.content.decode('UTF-8'))
+            return ""
+
+    def _PostMethod(self, url : str, data : str, sendSource=True):
+        if sendSource:
+            response = self.__requests.post(url, headers={
+                "Authorization": self.__constants.JSessionId,
+                "Source": self.__constants.ApiKey,
+                "SourceToken": self.__constants.VendorSession,
+                "AppIdKey": self.__constants.AppIdKey,
+                "Content-type": "application/json"}, data=data)
+
+        else:
+            response = self.__requests.post(url, headers={
+                "Authorization": self.__constants.JSessionId,
+                "SourceToken": self.__constants.VendorSession,
+                "AppIdKey": self.__constants.AppIdKey,
+                "Content-type": "application/json"}, data=data)
+
+        if response.headers.get('AppIdKey') != "":
+            self.__constants.AppIdKey = response.headers.get('AppIdKey')
+        if response.status_code == 200:
+            return json.loads(response.content)
+        else:
+            if 'Expired' in response.content.decode('UTF-8'):
+                print(json.dumps(json.loads(response.content.decode('UTF-8'))))
+                if path.exists(self.__constants.Filename):
+                    os.remove(self.__constants.Filename)
+                print("Expired session.")
+            self.LOGGER.debug("Error response: %s", response.content.decode('UTF-8'))
+            return ""
+
+    def _PutMethod(self, url : str, data : str):
+        response = self.__requests.put(url, headers={"Authorization": self.__constants.JSessionId,
+                                                "Source": self.__constants.ApiKey,
+                                                "SourceToken": self.__constants.VendorSession,
+                                                "AppIdKey": self.__constants.AppIdKey,
+                                                "Content-type": "application/json"}, data=data)
+        if response.headers.get('AppIdKey') != "":
+            self.__constants.AppIdKey = response.headers.get('AppIdKey')
+        if response.status_code == 200:
+            return json.loads(response.content)
+
+        else:
+            if 'Expired' in response.content.decode('UTF-8'):
+                if path.exists(self.__constants.Filename):
+                    os.remove(self.__constants.Filename)
+                print("Expired session.")
+            self.LOGGER.debug("Error response: %s", response.content.decode('UTF-8'))
+            return ""
+
+    def _DeleteMethod(self, url : str, data : str):
+        response = self.__requests.delete(url, headers={"Authorization": self.__constants.JSessionId,
+                                                    "Source": self.__constants.ApiKey,
+                                                    "SourceToken": self.__constants.VendorSession,
+                                                    "AppIdKey": self.__constants.AppIdKey,
+                                                    "Content-type": "application/json"}, data=data)
+        if response.headers.get('AppIdKey') != "":
+            self.__constants.AppIdKey = response.headers.get('AppIdKey')
+        if response.status_code == 200:
+            return json.loads(response.content)
+
+        else:
+            if 'Expired' in response.content.decode('UTF-8'):
+                if path.exists(self.__constants.Filename):
+                    os.remove(self.__constants.Filename)
+                print("Expired session.")
+            self.LOGGER.debug("Error response: %s", response.content.decode('UTF-8'))
+            return ""
+
+
```

### Comparing `APIConnect-2.0.1.post1/APIConnect/order.py` & `APIConnect-2.0.2/APIConnect/order.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-from constants.action import ActionEnum
-from constants.duration import DurationEnum
-from constants.exchange import ExchangeEnum
-from constants.order_type import OrderTypeEnum
-from constants.product_code import ProductCodeENum
-from APIConnect.validator import Validator
-
-
-class Order:
-
-    @Validator.ValidateInputDataTypes
-
-    def __init__(self, Exchange : ExchangeEnum, TradingSymbol, StreamingSymbol, Action : ActionEnum, ProductCode : ProductCodeENum,
-                 OrderType : OrderTypeEnum, Duration : DurationEnum, Price, TriggerPrice, Quantity : int, DisclosedQuantity,
-                 GTDDate, Remark):
-        '''
-
-         Exchange: Exchange of the scrip
-
-         TradingSymbol: Trading Symbol, to be obtained from Contract Notes
-
-         StreamingSymbol: ScripCode_exchange
-
-         Action: BUY/SELL
-
-         ProductCode: CNC/MIS/NRML
-
-         OrderType: LIMIT/MARKET
-
-         Duration: Validity DAY/IOC
-
-         Price: Limit price of the scrip
-
-         TriggerPrice: Trigger Price in case of SL/SL-M Order
-
-         Quantity: Quantity of scrip to be purchased
-
-         DisclosedQuantity: Disclosed Quantiy for the Order
-
-         GTDDate: Good Till Date in dd/MM/yyyy format
-
-         Remark: remark
-
-        '''
-        self.exc = Exchange
-        self.trdSym = TradingSymbol
-        self.sym = StreamingSymbol
-        self.action = Action
-        self.prdCode = ProductCode
-        self.ordTyp = OrderType
-        self.dur = Duration
-        self.price = Price
-        self.trgPrc = TriggerPrice
-        self.qty = Quantity
-        self.dscQty = DisclosedQuantity
-        self.GTDDate = GTDDate
-        self.rmk = Remark
-
-    def __str__(self) -> str:
-        return f'''ORDER DATA :
-    exc = {self.exc}
-    trdSym = {self.trdSym}
-    sym = {self.sym}
-    action = {self.action}
-    prdCode = {self.prdCode}
-    ordTyp = {self.ordTyp}
-    dur = {self.dur}
-    price = {self.price}
-    trgPrc = {self.trgPrc}
-    qty = {self.qty}
-    dscQty = {self.dscQty}
-    GTDDate = {self.GTDDate}
-    rmk = {self.rmk}'''
-
-    @property
-    def exc(self):
-        return self.__exc
-    @exc.setter
-    def exc(self, val):
-        self.__exc = val
-
-    @property
-    def trdSym(self):
-        return self.__trdSym
-    @trdSym.setter
-    def trdSym(self, val):
-        self.__trdSym = val
-
-    @property
-    def sym(self):
-        return self.__sym
-    @sym.setter
-    def sym(self, val):
-        self.__sym = val
-
-    @property
-    def action(self):
-        return self.__action
-    @action.setter
-    def action(self, val):
-        self.__action = val
-
-    @property
-    def prdCode(self):
-        return self.__prdCode
-    @prdCode.setter
-    def prdCode(self, val):
-        self.__prdCode = val
-
-    @property
-    def ordTyp(self):
-        return self.__ordTyp
-    @ordTyp.setter
-    def ordTyp(self, val):
-        self.__ordTyp = val
-
-    @property
-    def dur(self):
-        return self.__dur
-    @dur.setter
-    def dur(self, val):
-        self.__dur = val
-
-    @property
-    def price(self):
-        return self.__price
-    @price.setter
-    def price(self, val):
-        self.__price = val
-
-    @property
-    def trgPrc(self):
-        return self.__trgPrc
-    @trgPrc.setter
-    def trgPrc(self, val):
-        self.__trgPrc = val
-
-    @property
-    def qty(self):
-        return self.__qty
-    @qty.setter
-    def qty(self, val):
-        self.__qty = val
-
-    @property
-    def dscQty(self):
-        return self.__dscQty
-    @dscQty.setter
-    def dscQty(self, val):
-        self.__dscQty = val
-
-    @property
-    def GTDDate(self):
-        return self.__GTDDate
-    @GTDDate.setter
-    def GTDDate(self, val):
-        self.__GTDDate = val
-
-    @property
-    def rmk(self):
-        return self.__rmk
-    @rmk.setter
-    def rmk(self, val):
-        self.__rmk = val
+from constants.action import ActionEnum
+from constants.duration import DurationEnum
+from constants.exchange import ExchangeEnum
+from constants.order_type import OrderTypeEnum
+from constants.product_code import ProductCodeENum
+from APIConnect.validator import Validator
+
+
+class Order:
+
+    @Validator.ValidateInputDataTypes
+
+    def __init__(self, Exchange : ExchangeEnum, TradingSymbol, StreamingSymbol, Action : ActionEnum, ProductCode : ProductCodeENum,
+                 OrderType : OrderTypeEnum, Duration : DurationEnum, Price, TriggerPrice, Quantity : int, DisclosedQuantity,
+                 GTDDate, Remark):
+        '''
+
+         Exchange: Exchange of the scrip
+
+         TradingSymbol: Trading Symbol, to be obtained from Contract Notes
+
+         StreamingSymbol: ScripCode_exchange
+
+         Action: BUY/SELL
+
+         ProductCode: CNC/MIS/NRML
+
+         OrderType: LIMIT/MARKET
+
+         Duration: Validity DAY/IOC
+
+         Price: Limit price of the scrip
+
+         TriggerPrice: Trigger Price in case of SL/SL-M Order
+
+         Quantity: Quantity of scrip to be purchased
+
+         DisclosedQuantity: Disclosed Quantiy for the Order
+
+         GTDDate: Good Till Date in dd/MM/yyyy format
+
+         Remark: remark
+
+        '''
+        self.exc = Exchange
+        self.trdSym = TradingSymbol
+        self.sym = StreamingSymbol
+        self.action = Action
+        self.prdCode = ProductCode
+        self.ordTyp = OrderType
+        self.dur = Duration
+        self.price = Price
+        self.trgPrc = TriggerPrice
+        self.qty = Quantity
+        self.dscQty = DisclosedQuantity
+        self.GTDDate = GTDDate
+        self.rmk = Remark
+
+    def __str__(self) -> str:
+        return f'''ORDER DATA :
+    exc = {self.exc}
+    trdSym = {self.trdSym}
+    sym = {self.sym}
+    action = {self.action}
+    prdCode = {self.prdCode}
+    ordTyp = {self.ordTyp}
+    dur = {self.dur}
+    price = {self.price}
+    trgPrc = {self.trgPrc}
+    qty = {self.qty}
+    dscQty = {self.dscQty}
+    GTDDate = {self.GTDDate}
+    rmk = {self.rmk}'''
+
+    @property
+    def exc(self):
+        return self.__exc
+    @exc.setter
+    def exc(self, val):
+        self.__exc = val
+
+    @property
+    def trdSym(self):
+        return self.__trdSym
+    @trdSym.setter
+    def trdSym(self, val):
+        self.__trdSym = val
+
+    @property
+    def sym(self):
+        return self.__sym
+    @sym.setter
+    def sym(self, val):
+        self.__sym = val
+
+    @property
+    def action(self):
+        return self.__action
+    @action.setter
+    def action(self, val):
+        self.__action = val
+
+    @property
+    def prdCode(self):
+        return self.__prdCode
+    @prdCode.setter
+    def prdCode(self, val):
+        self.__prdCode = val
+
+    @property
+    def ordTyp(self):
+        return self.__ordTyp
+    @ordTyp.setter
+    def ordTyp(self, val):
+        self.__ordTyp = val
+
+    @property
+    def dur(self):
+        return self.__dur
+    @dur.setter
+    def dur(self, val):
+        self.__dur = val
+
+    @property
+    def price(self):
+        return self.__price
+    @price.setter
+    def price(self, val):
+        self.__price = val
+
+    @property
+    def trgPrc(self):
+        return self.__trgPrc
+    @trgPrc.setter
+    def trgPrc(self, val):
+        self.__trgPrc = val
+
+    @property
+    def qty(self):
+        return self.__qty
+    @qty.setter
+    def qty(self, val):
+        self.__qty = val
+
+    @property
+    def dscQty(self):
+        return self.__dscQty
+    @dscQty.setter
+    def dscQty(self, val):
+        self.__dscQty = val
+
+    @property
+    def GTDDate(self):
+        return self.__GTDDate
+    @GTDDate.setter
+    def GTDDate(self, val):
+        self.__GTDDate = val
+
+    @property
+    def rmk(self):
+        return self.__rmk
+    @rmk.setter
+    def rmk(self, val):
+        self.__rmk = val
```

### Comparing `APIConnect-2.0.1.post1/APIConnect/validator.py` & `APIConnect-2.0.2/APIConnect/validator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,109 +1,119 @@
-from datetime import datetime
-import functools
-import inspect
-import logging
-from exceptions.validation_exception import ValidationException
-
-LOGGER = logging.getLogger(__name__)
-
-class Validator:
-
-    # validation decorator
-    @staticmethod
-    def ValidateInputDataTypes(func):
-        @functools.wraps(func)
-        def validate(*args, **kwargs):
-            # a mapping of variable names from the function definition and the values given at function call time
-            variables_value_map = dict(inspect.signature(func).bind(*args, **kwargs).arguments)
-
-            # a mapping of variables and their type annotations provided in function defintion
-            for variable, type_annotation in func.__annotations__.items():
-                if variable not in variables_value_map.keys():
-                    # if some option variable is not given a value at function call time, skip its type checking
-                    continue
-                if type_annotation in [None, True, False]:
-                    type_annotation = type(type_annotation)
-                if not isinstance(variables_value_map[variable], type_annotation):
-                    exc = ValidationException(f"Function {func.__name__} : {variable} is a not a valid {type_annotation} type.")
-                    LOGGER.exception(exc)
-                    raise exc
-            return func(*args, **kwargs)
-        return validate
-
-    # isRequired decorator
-    @staticmethod
-    def isRequired(required=None):
-        '''
-        Parameters :
-        `required` : Name of parameter as a string | List of strings of parameter names
-        '''
-        def is_none_or_empty_test(func, args_dict, required):
-            has_none_is_empty = False
-            bad_parameters = []
-
-            for param, value in args_dict.items():
-                if param in list(required):
-                    if isinstance(value, str):
-                        value = value.strip()
-                    try:
-                        len(value)
-                    except TypeError as e:
-                        # TypeError if value is of type <int/float or None or something else> - numerics are currently allowed to be 0
-                        if value is None:
-                            bad_parameters.append(param)
-                            has_none_is_empty = True
-                    else:
-                        if not len(value):
-                            # checks for empty <strings, dicts, lists, tuples>
-                            bad_parameters.append(param)
-                            has_none_is_empty = True
-
-            if has_none_is_empty:
-                exc = ValidationException(
-                    f'function {func.__name__}: Parameters {bad_parameters} cannot be None or Empty.')
-                LOGGER.exception(exc)
-                raise exc
-
-        def real_decorator(func):
-            @functools.wraps(func)
-            def wrapper(*args, **kwargs):
-                variables_value_map = dict(
-                    zip(inspect.signature(func).parameters, args+tuple(kwargs.values())))
-                is_none_or_empty_test(func, variables_value_map, required)
-                return func(*args, **kwargs)
-            return wrapper
-        return real_decorator
-
-    @staticmethod
-    def isRequiredv2(name, value):
-
-        has_none_is_empty = False
-
-        if isinstance(value, str):
-            value = value.strip()
-        try:
-            len(value)
-        except TypeError as e:
-            # TypeError if value is of type <int/float or None or something else> - numerics are currently allowed to be 0
-            if value is None:
-                has_none_is_empty = True
-        else:
-            if not len(value):
-                # checks for empty <strings, dicts, lists, tuples>
-                has_none_is_empty = True
-
-        if has_none_is_empty:
-            exc = ValidationException(f'Parameter {name} cannot be None or Empty.')
-            LOGGER.exception(exc)
-            raise exc
-
-        return value
-
-    @staticmethod
-    def validate_datetime_format(date_time_string, pattern) :
-        try:
-            datetime.strptime(date_time_string, pattern)
-        except ValueError as e:
-            exc = ValidationException(e.args[0])
-            LOGGER.exception(exc)
-            raise exc
+import functools
+import inspect
+import logging
+from datetime import datetime
+
+from exceptions.validation_exception import ValidationException
+
+LOGGER = logging.getLogger(__name__)
+
+class Validator:
+
+    # validation decorator
+    @staticmethod
+    def ValidateInputDataTypes(func):
+        @functools.wraps(func)
+        def validate(*args, **kwargs):
+            # a mapping of variable names from the function definition and the values given at function call time
+            variables_value_map = dict(inspect.signature(func).bind(*args, **kwargs).arguments)
+
+            # a mapping of variables and their type annotations provided in function defintion
+            for variable, type_annotation in func.__annotations__.items():
+                if variable not in variables_value_map.keys():
+                    # if some optional variable is not given a value at function call time, skip its type checking
+                    continue
+                if type_annotation in [None, True, False]:
+                    type_annotation = type(type_annotation)
+                if not isinstance(variables_value_map[variable], type_annotation):
+                    exc = ValidationException(f"Function {func.__name__} : '{variables_value_map[variable]}' is not a valid {type_annotation} type.")
+                    LOGGER.exception(exc)
+                    raise exc
+            return func(*args, **kwargs)
+        return validate
+
+    # isRequired decorator
+    @staticmethod
+    def isRequired(required=None):
+        '''
+        Parameters :
+        `required` : Name of parameter as a string | List of strings of parameter names
+        '''
+        def is_none_or_empty_test(func, args_dict, required):
+            has_none_is_empty = False
+            bad_parameters = []
+
+            for param, value in args_dict.items():
+                if param in list(required):
+                    if isinstance(value, str):
+                        value = value.strip()
+                    try:
+                        len(value)
+                    except TypeError as e:
+                        # TypeError if value is of type <int/float or None or something else> - numerics are currently allowed to be 0
+                        if value is None:
+                            bad_parameters.append(param)
+                            has_none_is_empty = True
+                    else:
+                        if not len(value):
+                            # checks for empty <strings, dicts, lists, tuples>
+                            bad_parameters.append(param)
+                            has_none_is_empty = True
+
+            if has_none_is_empty:
+                exc = ValidationException(
+                    f'function {func.__name__}: Parameters {bad_parameters} cannot be None or Empty.')
+                LOGGER.exception(exc)
+                raise exc
+
+        def real_decorator(func):
+            @functools.wraps(func)
+            def wrapper(*args, **kwargs):
+                variables_value_map = dict(
+                    zip(inspect.signature(func).parameters, args+tuple(kwargs.values())))
+                is_none_or_empty_test(func, variables_value_map, required)
+                return func(*args, **kwargs)
+            return wrapper
+        return real_decorator
+
+    @staticmethod
+    def isRequiredv2(name, value):
+
+        has_none_is_empty = False
+
+        if isinstance(value, str):
+            value = value.strip()
+        try:
+            len(value)
+        except TypeError as e:
+            # TypeError if value is of type <int/float or None or something else> - numerics are currently allowed to be 0
+            if value is None:
+                has_none_is_empty = True
+        else:
+            if not len(value):
+                # checks for empty <strings, dicts, lists, tuples>
+                has_none_is_empty = True
+
+        if has_none_is_empty:
+            exc = ValidationException(f'Parameter {name} cannot be None or Empty.')
+            LOGGER.exception(exc)
+            raise exc
+
+        return value
+
+    @staticmethod
+    def validate_datetime_format(date_time_string, pattern) :
+        try:
+            datetime.strptime(date_time_string, pattern)
+        except ValueError as e:
+            exc = ValidationException(e.args[0])
+            LOGGER.exception(exc)
+            raise exc
+
+    @staticmethod
+    def product_code(prd_code : str, exchange : str, exch_prdcode_map : dict) -> str:
+        try :
+            return exch_prdcode_map[prd_code][exchange]
+        except KeyError:
+            e = ValidationException(f"Product Code '{prd_code}' is not available for exchange '{exchange}'.")
+            LOGGER.exception(e)
+            raise e
```

### Comparing `APIConnect-2.0.1.post1/APIConnect.egg-info/PKG-INFO` & `APIConnect-2.0.2/APIConnect.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-Metadata-Version: 2.1
-Name: APIConnect
-Version: 2.0.1.post1
-Summary: APIs to trade from Nuvama
-Home-page: https://nuvamawealth.com/
-Author: Nuvama
-Author-email: support@nuvama.com
-License: MIT
-Download-URL: https://www.nuvamawealth.com/ewwebimages/webfiles/download/Python_APIConnect/APIConnect-2.0.1.post1.tar.gz
-Keywords: Nuvama,Open API,Trade,Nuvama Python Library
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.7
-License-File: LICENSE.txt
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: APIConnect
+Version: 2.0.2
+Summary: APIs to trade from Nuvama
+Home-page: https://nuvamawealth.com/
+Download-URL: https://www.nuvamawealth.com/ewwebimages/webfiles/download/Python_APIConnect/APIConnect-2.0.2.tar.gz
+Author: Nuvama
+Author-email: support@nuvama.com
+License: MIT
+Keywords: Nuvama,Open API,Trade,Nuvama Python Library
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.7
+License-File: LICENSE.txt
```

### Comparing `APIConnect-2.0.1.post1/LICENSE.txt` & `APIConnect-2.0.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-MIT License
-Copyright (c) 2022 Nuvama Wealth and Investment Limited (NWIL), formerly known as Edelweiss Broking Limited
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+Copyright (c) 2022 Nuvama Wealth and Investment Limited (NWIL), formerly known as Edelweiss Broking Limited
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `APIConnect-2.0.1.post1/PKG-INFO` & `APIConnect-2.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-Metadata-Version: 2.1
-Name: APIConnect
-Version: 2.0.1.post1
-Summary: APIs to trade from Nuvama
-Home-page: https://nuvamawealth.com/
-Author: Nuvama
-Author-email: support@nuvama.com
-License: MIT
-Download-URL: https://www.nuvamawealth.com/ewwebimages/webfiles/download/Python_APIConnect/APIConnect-2.0.1.post1.tar.gz
-Keywords: Nuvama,Open API,Trade,Nuvama Python Library
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.7
-License-File: LICENSE.txt
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: APIConnect
+Version: 2.0.2
+Summary: APIs to trade from Nuvama
+Home-page: https://nuvamawealth.com/
+Download-URL: https://www.nuvamawealth.com/ewwebimages/webfiles/download/Python_APIConnect/APIConnect-2.0.2.tar.gz
+Author: Nuvama
+Author-email: support@nuvama.com
+License: MIT
+Keywords: Nuvama,Open API,Trade,Nuvama Python Library
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.7
+License-File: LICENSE.txt
```

### Comparing `APIConnect-2.0.1.post1/constants/constants.py` & `APIConnect-2.0.2/constants/constants.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from enum import Enum, unique
-
-
-@unique
-class BaseUrl(str, Enum) :
-    '''
-    Enum class for all the allowed types of Orders.
-    '''
-    BASE_EQ = "https://nc.nuvamawealth.com/edelmw-eq/eq/"
-    BASE_COMM = "https://nc.nuvamawealth.com/edelmw-comm/comm/"
-    BASE_CONTENT = "https://nc.nuvamawealth.com/edelmw-content/content/"
-    BASE_LOGIN = "https://nc.nuvamawealth.com/edelmw-login/login/"
-    BASE_MF_LOGIN = "https://nc.nuvamawealth.com/edelmw-mf/mf/"
-    EQ_CONTRACT = "https://nc.nuvamawealth.com/app/toccontracts/instruments.zip"
+from enum import Enum, unique
+
+
+@unique
+class BaseUrl(str, Enum) :
+    '''
+    Enum class for all the allowed types of Orders.
+    '''
+    BASE_EQ = "https://nc.nuvamawealth.com/edelmw-eq/eq/"
+    BASE_COMM = "https://nc.nuvamawealth.com/edelmw-comm/comm/"
+    BASE_CONTENT = "https://nc.nuvamawealth.com/edelmw-content/content/"
+    BASE_LOGIN = "https://nc.nuvamawealth.com/edelmw-login/login/"
+    BASE_MF_LOGIN = "https://nc.nuvamawealth.com/edelmw-mf/mf/"
+    EQ_CONTRACT = "https://nc.nuvamawealth.com/app/toccontracts/instruments.zip"
     MF_CONTRACT = "https://nc.nuvamawealth.com/app/toccontracts/mfInstruments.zip"
```

### Comparing `APIConnect-2.0.1.post1/constants/router.py` & `APIConnect-2.0.2/constants/router.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,223 +1,206 @@
-import logging
-from constants.constants import BaseUrl
-import urllib
-
-class Router:
-
-    def __init__(self, config_obj=None):
-
-        self.LOGGER = logging.getLogger(__name__)
-        self.LOGGER.info("Router object is being created.")
-
-        self.baseurleq = BaseUrl.BASE_EQ.value
-        self.baseurlcomm = BaseUrl.BASE_COMM.value
-        self.baseurlcontent = BaseUrl.BASE_CONTENT.value
-        self.baseurllogin = BaseUrl.BASE_LOGIN.value
-        self.basemflogin = BaseUrl.BASE_MF_LOGIN.value
-        self.EquityContractURL = BaseUrl.EQ_CONTRACT.value
-        self.MFContractURL = BaseUrl.MF_CONTRACT.value
-
-        if config_obj and 'GLOBAL' in config_obj:
-            if config_obj['GLOBAL'].get('BasePathLogin'):
-                self.baseurllogin = config_obj['GLOBAL']['BasePathLogin']
-            if config_obj['GLOBAL'].get('BasePathEq'):
-                self.baseurleq = config_obj['GLOBAL']['BasePathEq']
-            if config_obj['GLOBAL'].get('BasePathComm'):
-                self.baseurlcomm = config_obj['GLOBAL']['BasePathComm']
-            if config_obj['GLOBAL'].get('BasePathMf'):
-                self.basemflogin = config_obj['GLOBAL']['BasePathMf']
-            if config_obj['GLOBAL'].get('BasePathContent'):
-                self.baseurlcontent = config_obj['GLOBAL']['BasePathContent']
-            if config_obj['GLOBAL'].get('EquityContractURL'):
-                self.EquityContractURL = config_obj['GLOBAL']['EquityContractURL']
-            if config_obj['GLOBAL'].get('MFContractURL'):
-                self.MFContractURL = config_obj['GLOBAL']['MFContractURL']
-            if config_obj['GLOBAL'].get('AppIdKey'):
-                self._AppIdKey = config_obj['GLOBAL']['AppIdKey']
-            self.LOGGER.info("URL constants loaded with provided configuration file.")
-
-    def _CheckUpdateURl(self):
-        return urllib.parse.urljoin(self.baseurlcontent, "adhoc/lib/version/")
-
-    def _OrderBookURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "order/book/{userid}/v1/")
-
-    def _OrderBookURL_comm(self):
-        return urllib.parse.urljoin(self.baseurlcomm, "orderbook/{userid}?rTyp={reqtype}/")
-
-    def _TradeBookURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "tradebook/v1/{userid}/")
-
-    def _TradeBookURL_comm(self):
-        return urllib.parse.urljoin(self.baseurlcomm, "tradebook/{userid}/")
-
-    def _NetPositionURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "positions/net/{userid}/")
-
-    def _NetPositionURL_comm(self):
-        return urllib.parse.urljoin(self.baseurlcomm, "positions/{userid}/")
-
-    def _PlaceTradeURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/placetrade/{userid}/")
-
-    def _PlaceTradeURL_comm(self):
-        return urllib.parse.urljoin(self.baseurlcomm, "trade/placetrade/{userid}/")
-
-    def _PlaceBracketTradeURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/placebrackettrade/{userid}/")
-
-    def _PlaceCoverTradeURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/covertrade/{userid}/")
-
-    def _ModifyCoverTradeURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/modifycovertrade/{userid}/")
-
-    def _ExitCoverTradeURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/exitcovertrade/{userid}/")
-
-    def _PlaceBasketTradeURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/basketorder/{userid}/")
-
-    def _ExitBracketTradeURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/exitbrackettrade/{userid}/")
-
-    def _PlaceGtcGtdTradeURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/placegtcgtdtrade/{userid}/")
-
-    def _PlaceGtcGtdTradeURL_comm(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/placegtcgtdtrade/{userid}/")
-
-    def _OrderDetailsURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "order/details/{userid}?nOID={orderid}")
-
-    def _OrderDetailsURL_comm(self):
-        return urllib.parse.urljoin(self.baseurlcomm, "orderdetails/{userid}?oID={orderid}")
-
-    def _OrderHistoryURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "order/history/{userid}?sDt={StartDate}&eDt={EndDate}/")
-
-    def _OrderHistoryURL_comm(self):
-        return urllib.parse.urljoin(self.baseurlcomm, "orderhistory/{userid}?sDt={StartDate}&eDt={EndDate}/")
-
-    def _ModifyTradeURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/modifytrade/{userid}/")
-
-    def _ModifyTradeURL_comm(self):
-        return urllib.parse.urljoin(self.baseurlcomm, "trade/modifytrade/{userid}/")
-
-    def _CancelTradeURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/canceltrade/v1/{userid}/")
-
-    def _CancelTradeURL_comm(self):
-        return urllib.parse.urljoin(self.baseurlcomm, "trade/canceltrade/v1/{userid}/")
-
-    def _HoldingURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "holdings/v1/rmsholdings/{userid}/")
-
-    def _HoldingURL_comm(self):
-        return urllib.parse.urljoin(self.baseurlcomm, "reports/detail/{userid}/")
-
-    def _LimitsURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "limits/rmssublimits/{userid}/")
-
-    def _LimitsURL_comm(self):
-        return urllib.parse.urljoin(self.baseurlcomm, "limits/{userid}/")
-
-    def _GetAMOFlag(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/amoflag/")
-
-    def _GetAMOFlag_comm(self):
-        return urllib.parse.urljoin(self.baseurlcomm, "trade/amoflag/")
-
-    def _PositionSqOffURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/position/sqroff/{userid}/")
-
-    def _ConvertPositionURL(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/convertposition/v1/{userid}/")
-
-    def _ConvertPositionURL_comm(self):
-        return urllib.parse.urljoin(self.baseurlcomm, "trade/convertposition/v1/{userid}/")
-
-    def _PlaceAMOTrade(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/amo/placetrade/{userid}/")
-
-    def _PlaceAMOTrade_comm(self):
-        return urllib.parse.urljoin(self.baseurlcomm, "trade/amo/placetrade/{userid}/")
-
-    def _ModifyAMOTrade(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/amo/modifytrade/{userid}/")
-
-    def _ModifyAMOTrade_comm(self):
-        return urllib.parse.urljoin(self.baseurlcomm, "trade/amo/modifytrade/{userid}/")
-
-    def _CancelAMOTrade(self):
-        return urllib.parse.urljoin(self.baseurleq, "trade/amo/canceltrade/v1/{userid}/")
-
-    def _CancelAMOTrade_comm(self):
-        return urllib.parse.urljoin(self.baseurlcomm, "trade/amo/canceltrade/v1/{userid}/")
-
-    # MF Related APIs
-
-    def _PlaceMFURL(self):
-        return urllib.parse.urljoin(self.basemflogin, "trade/{userid}/")
-
-    def _ModifyMFURL(self):
-        return urllib.parse.urljoin(self.basemflogin, "trade/{userid}/")
-
-    def _CancelMFURL(self):
-        return urllib.parse.urljoin(self.basemflogin, "trade/{userid}/")
-
-    def _HoldingsMFURL(self):
-        return urllib.parse.urljoin(self.basemflogin, "holding/{userid}/")
-
-    def _OrderBookMFURL(self):
-        return urllib.parse.urljoin(self.basemflogin, "order/{userid}?frDt={fromDate}&toDt={toDate}/")
-
-    # Charts Related APIs
-
-    def _ChartsURL(self):
-        return urllib.parse.urljoin(self.baseurlcontent, "charts/v2/main/{interval}/{exc}/{aTyp}/{symbol}")
-
-    # Live News related APIs
-
-    def _LiveNewsCategoriesURL(self) -> str:
-        return urllib.parse.urljoin(self.baseurlcontent, "liveNews/getfiltersandcatagories")
-
-    def _GeneralNewsURL(self) -> str:
-        return urllib.parse.urljoin(self.baseurlcontent, "liveNews/general")
-
-    def _HoldingsNewsURL(self) -> str :
-        return urllib.parse.urljoin(self.baseurleq, "news/eqholdings")
-
-    def _LatestCorpActionsURL(self) -> str :
-        return urllib.parse.urljoin(self.baseurlcontent, "events/latestcorpactions/{symbol}")
-
-    # Watchlist related APIs
-
-    def _WatchlistBaseGroupsURL(self):
-        return urllib.parse.urljoin(self.baseurlcontent, "accounts/groups")
-
-    def _WatchlistGetScripsURL(self):
-        return urllib.parse.urljoin(self.baseurlcontent, "accounts/groups/symbols")
-
-    def _WatchlistGroupNameURL(self):
-        return urllib.parse.urljoin(self.baseurlcontent, "accounts/groups/{groupName}/")
-
-    # Research Calls related APIs
-
-    def _ActiveResearchCallsURL(self):
-        return urllib.parse.urljoin(self.baseurlcontent, "research/active")
-
-    def _ClosedResearchCallsURL(self):
-        return urllib.parse.urljoin(self.baseurlcontent, "research/closed")
-
-    # Login related APIs
-
-    def _LoginURL(self):
-        return urllib.parse.urljoin(self.baseurllogin, "accounts/loginvendor/{vendorId}/")
-
-    def _TokenURL(self):
-        return urllib.parse.urljoin(self.baseurllogin, "accounts/logindata/")
-
-    def _LogoutURL(self):
-        return urllib.parse.urljoin(self.baseurllogin, "accounts/{userid}/logout/")
+import logging
+from constants.constants import BaseUrl
+import urllib
+
+class Router:
+
+    def __init__(self, config_obj=None):
+
+        self.LOGGER = logging.getLogger(__name__)
+        self.LOGGER.info("Router object is being created.")
+
+        self.baseurleq = BaseUrl.BASE_EQ.value
+        self.baseurlcomm = BaseUrl.BASE_COMM.value
+        self.baseurlcontent = BaseUrl.BASE_CONTENT.value
+        self.baseurllogin = BaseUrl.BASE_LOGIN.value
+        self.basemflogin = BaseUrl.BASE_MF_LOGIN.value
+        self.EquityContractURL = BaseUrl.EQ_CONTRACT.value
+        self.MFContractURL = BaseUrl.MF_CONTRACT.value
+
+        if config_obj and 'GLOBAL' in config_obj:
+            if config_obj['GLOBAL'].get('BasePathLogin'):
+                self.baseurllogin = config_obj['GLOBAL']['BasePathLogin']
+            if config_obj['GLOBAL'].get('BasePathEq'):
+                self.baseurleq = config_obj['GLOBAL']['BasePathEq']
+            if config_obj['GLOBAL'].get('BasePathComm'):
+                self.baseurlcomm = config_obj['GLOBAL']['BasePathComm']
+            if config_obj['GLOBAL'].get('BasePathMf'):
+                self.basemflogin = config_obj['GLOBAL']['BasePathMf']
+            if config_obj['GLOBAL'].get('BasePathContent'):
+                self.baseurlcontent = config_obj['GLOBAL']['BasePathContent']
+            if config_obj['GLOBAL'].get('EquityContractURL'):
+                self.EquityContractURL = config_obj['GLOBAL']['EquityContractURL']
+            if config_obj['GLOBAL'].get('MFContractURL'):
+                self.MFContractURL = config_obj['GLOBAL']['MFContractURL']
+            if config_obj['GLOBAL'].get('AppIdKey'):
+                self._AppIdKey = config_obj['GLOBAL']['AppIdKey']
+            self.LOGGER.info("URL constants loaded with provided configuration file.")
+
+    def _CheckUpdateURl(self):
+        return urllib.parse.urljoin(self.baseurlcontent, "adhoc/lib/version/")
+
+    def _OrderBookURL(self):
+        return urllib.parse.urljoin(self.baseurleq, "order/book/{userid}/v1/")
+
+    def _OrderBookURL_comm(self):
+        return urllib.parse.urljoin(self.baseurlcomm, "orderbook/{userid}?rTyp={reqtype}/")
+
+    def _TradeBookURL(self):
+        return urllib.parse.urljoin(self.baseurleq, "tradebook/v1/{userid}/")
+
+    def _TradeBookURL_comm(self):
+        return urllib.parse.urljoin(self.baseurlcomm, "tradebook/{userid}/")
+
+    def _NetPositionURL(self):
+        return urllib.parse.urljoin(self.baseurleq, "positions/net/{userid}/")
+
+    def _NetPositionURL_comm(self):
+        return urllib.parse.urljoin(self.baseurlcomm, "positions/{userid}/")
+
+    def _PlaceTradeURL(self):
+        return urllib.parse.urljoin(self.baseurleq, "trade/placetrade/{userid}/")
+
+    def _PlaceTradeURL_comm(self):
+        return urllib.parse.urljoin(self.baseurlcomm, "trade/placetrade/{userid}/")
+
+    def _PlaceBracketTradeURL(self):
+        return urllib.parse.urljoin(self.baseurleq, "trade/placebrackettrade/{userid}/")
+
+    def _PlaceBasketTradeURL(self):
+        return urllib.parse.urljoin(self.baseurleq, "trade/basketorder/{userid}/")
+
+    def _ExitBracketTradeURL(self):
+        return urllib.parse.urljoin(self.baseurleq, "trade/exitbrackettrade/{userid}/")
+
+    def _PlaceGtcGtdTradeURL(self):
+        return urllib.parse.urljoin(self.baseurleq, "trade/placegtcgtdtrade/{userid}/")
+
+    def _PlaceGtcGtdTradeURL_comm(self):
+        return urllib.parse.urljoin(self.baseurleq, "trade/placegtcgtdtrade/{userid}/")
+
+    def _OrderDetailsURL(self):
+        return urllib.parse.urljoin(self.baseurleq, "order/details/{userid}?nOID={orderid}")
+
+    def _OrderDetailsURL_comm(self):
+        return urllib.parse.urljoin(self.baseurlcomm, "orderdetails/{userid}?oID={orderid}")
+
+    def _OrderHistoryURL(self):
+        return urllib.parse.urljoin(self.baseurleq, "order/history/{userid}?sDt={StartDate}&eDt={EndDate}/")
+
+    def _OrderHistoryURL_comm(self):
+        return urllib.parse.urljoin(self.baseurlcomm, "orderhistory/{userid}?sDt={StartDate}&eDt={EndDate}/")
+
+    def _ModifyTradeURL(self):
+        return urllib.parse.urljoin(self.baseurleq, "trade/modifytrade/{userid}/")
+
+    def _ModifyTradeURL_comm(self):
+        return urllib.parse.urljoin(self.baseurlcomm, "trade/modifytrade/{userid}/")
+
+    def _CancelTradeURL(self):
+        return urllib.parse.urljoin(self.baseurleq, "trade/canceltrade/v1/{userid}/")
+
+    def _CancelTradeURL_comm(self):
+        return urllib.parse.urljoin(self.baseurlcomm, "trade/canceltrade/v1/{userid}/")
+
+    def _HoldingURL(self):
+        return urllib.parse.urljoin(self.baseurleq, "holdings/v1/rmsholdings/{userid}/")
+
+    def _HoldingURL_comm(self):
+        return urllib.parse.urljoin(self.baseurlcomm, "reports/detail/{userid}/")
+
+    def _LimitsURL(self):
+        return urllib.parse.urljoin(self.baseurleq, "limits/rmssublimits/{userid}/")
+
+    def _LimitsURL_comm(self):
+        return urllib.parse.urljoin(self.baseurlcomm, "limits/{userid}/")
+
+    def _GetAMOFlag(self):
+        return urllib.parse.urljoin(self.baseurleq, "trade/amoflag/")
+
+    def _GetAMOFlag_comm(self):
+        return urllib.parse.urljoin(self.baseurlcomm, "trade/amostatus/{exch}")
+
+    def _PositionSqOffURL(self):
+        return urllib.parse.urljoin(self.baseurleq, "trade/position/sqroff/{userid}/")
+
+    def _ConvertPositionURL(self):
+        return urllib.parse.urljoin(self.baseurleq, "trade/convertposition/v1/{userid}/")
+
+    def _ConvertPositionURL_comm(self):
+        return urllib.parse.urljoin(self.baseurlcomm, "trade/positionconversion/{userid}/")
+
+    def _PlaceAMOTrade(self):
+        return urllib.parse.urljoin(self.baseurleq, "trade/amo/placetrade/{userid}/")
+
+    def _PlaceAMOTrade_comm(self):
+        return urllib.parse.urljoin(self.baseurlcomm, "trade/amo/placetrade/{userid}/")
+
+    def _ModifyAMOTrade(self):
+        return urllib.parse.urljoin(self.baseurleq, "trade/amo/modifytrade/{userid}/")
+
+    def _ModifyAMOTrade_comm(self):
+        return urllib.parse.urljoin(self.baseurlcomm, "trade/amo/modifytrade/{userid}/")
+
+    def _CancelAMOTrade(self):
+        return urllib.parse.urljoin(self.baseurleq, "trade/amo/canceltrade/v1/{userid}/")
+
+    def _CancelAMOTrade_comm(self):
+        return urllib.parse.urljoin(self.baseurlcomm, "trade/amo/canceltrade/v1/{userid}/")
+
+    # MF Related APIs
+
+    def _PlaceMFURL(self):
+        return urllib.parse.urljoin(self.basemflogin, "trade/{userid}/")
+
+    def _ModifyMFURL(self):
+        return urllib.parse.urljoin(self.basemflogin, "trade/{userid}/")
+
+    def _CancelMFURL(self):
+        return urllib.parse.urljoin(self.basemflogin, "trade/{userid}/")
+
+    def _HoldingsMFURL(self):
+        return urllib.parse.urljoin(self.basemflogin, "holding/{userid}/")
+
+    def _OrderBookMFURL(self):
+        return urllib.parse.urljoin(self.basemflogin, "order/{userid}?frDt={fromDate}&toDt={toDate}/")
+
+    # Charts Related APIs
+
+    def _ChartsURL(self):
+        return urllib.parse.urljoin(self.baseurlcontent, "charts/v2/main/{interval}/{exc}/{aTyp}/{symbol}")
+
+    # Live News related APIs
+
+    def _LiveNewsCategoriesURL(self) -> str:
+        return urllib.parse.urljoin(self.baseurlcontent, "liveNews/getfiltersandcatagories")
+
+    def _GeneralNewsURL(self) -> str:
+        return urllib.parse.urljoin(self.baseurlcontent, "liveNews/general")
+
+    def _HoldingsNewsURL(self) -> str :
+        return urllib.parse.urljoin(self.baseurleq, "news/eqholdings")
+
+    def _LatestCorpActionsURL(self) -> str :
+        return urllib.parse.urljoin(self.baseurlcontent, "events/latestcorpactions/{symbol}")
+
+    # Watchlist related APIs
+
+    def _WatchlistBaseGroupsURL(self):
+        return urllib.parse.urljoin(self.baseurlcontent, "accounts/groups")
+
+    def _WatchlistGetScripsURL(self):
+        return urllib.parse.urljoin(self.baseurlcontent, "accounts/groups/symbols")
+
+    def _WatchlistGroupNameURL(self):
+        return urllib.parse.urljoin(self.baseurlcontent, "accounts/groups/{groupName}/")
+
+    # Login related APIs
+
+    def _LoginURL(self):
+        return urllib.parse.urljoin(self.baseurllogin, "accounts/loginvendor/{vendorId}/")
+
+    def _TokenURL(self):
+        return urllib.parse.urljoin(self.baseurllogin, "accounts/logindata/")
+
+    def _LogoutURL(self):
+        return urllib.parse.urljoin(self.baseurllogin, "account/logoff/{userid}/")
```

### Comparing `APIConnect-2.0.1.post1/feed/feed.py` & `APIConnect-2.0.2/feed/feed.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-from cgitb import Hook
-import json
-import logging
-import socket
-from threading import Thread
-from time import sleep
-from typing import Any, Callable
-
-from constants.streaming_constants import StreamingConstants
-
-LOGGER = logging.getLogger(__name__)
-
-class Feed:
-
-    def __init__(self, confObj):
-        self.__conf = confObj
-
-        AppIdKey = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhcHAiOjAsImZmIjoiVyIsImJkIjoid2ViLXBjIiwibmJmIjoxNjcxMTcwMjc2LCJzcmMiOiJlbXRtdyIsImF2IjoiMi4wLjAiLCJhcHBpZCI6IjQxZGE0MDEyNDg2YjFhY2IzNTc4YzYwZjdmNGUyNDhhIiwiaXNzIjoiZW10IiwiZXhwIjoxNjcxMjE1NDAwLCJpYXQiOjE2NzExNzA1NzZ9.7mqgyIfCxuILFGKI_WR0QsrS64mUIKptW5D7utHyDHA"
-        Host="ncst.nuvamawealth.com"
-        Port=9443
-
-        self._appID = AppIdKey
-        self.__host = Host
-        self.__port = Port
-
-        if self.__conf:
-            if self.__conf['GLOBAL'].get('AppIdKey'):
-                self._appID = self.__conf['GLOBAL'].get('AppIdKey')
-            if self.__conf['STREAM'].get('HOST'):
-                self.__host = self.__conf['STREAM'].get('HOST')
-            if self.__conf['STREAM'].get('PORT'):
-                self.__port = int(self.__conf['STREAM'].get('PORT'))
-        self._sock = None
-        self._socket_fs = None
-        self.__requestsList = {}
-
-        t = Thread(target=self.__do_connection)
-        t.start()
-
-    def _subscribe(self, request : str, callback : Callable[[str], Any], requestCode : StreamingConstants):
-        self.__requestsList[requestCode] = {'request' : request, 'callback' : callback}
-        self.__sub(requestCode)
-
-    def _unsubscribe(self, request : str, requestCode : StreamingConstants):
-        if self.__is_connection_alive():
-            self.__send_stream_request(request)
-        else :
-            self.__do_connection()
-            self.__send_stream_request(request)
-        self.__requestsList.pop(requestCode, "Key not found")
-
-
-    def __sub(self, action):
-        if self.__is_connection_alive():
-            if action == 'all':
-                for req_code in self.__requestsList.keys():
-                    self.__start_streaming(self.__requestsList[req_code]['request'])
-                    sleep(0.1)
-            elif type(action) is StreamingConstants:
-                self.__start_streaming(self.__requestsList[action]['request'])
-        else:
-            self.__do_connection()
-            self.__sub(action)
-
-    def __start_streaming(self, sendRequest : str):
-        self.__send_stream_request(sendRequest)
-        t_read = Thread(target = self.__read_stream_data)
-        t_read.start()
-
-    def __send_stream_request(self, request : str):
-        self._socket_fs.writelines(request)
-        self._socket_fs.flush()
-
-    def __read_stream_data(self):
-        while True:
-            resp = self._socket_fs.readline()
-
-            if resp:
-                LOGGER.debug(f"Response recevied : {resp}")
-                try:
-                    resp_dict = json.loads(resp)
-
-                    if resp_dict['response']["streaming_type"] == "quote3":
-                        callback = self.__requestsList[StreamingConstants.QUOTE_SREAM_REQ_CODE]['callback']
-                    elif resp_dict['response']["streaming_type"] == "orderFiler":
-                        callback = self.__requestsList[StreamingConstants.ORDER_STREAM_REQ_CODE]['callback']
-                    elif resp_dict['response']["streaming_type"] == "news":
-                        callback = self.__requestsList[StreamingConstants.LIVENEWS_STREAM_REQ_CODE]['callback']
-
-                    callback(resp)
-
-                except json.JSONDecodeError:
-                    pass
-
-            else:
-                LOGGER.error("Response Blank. Socket Connection seems to be closed. Trying to reconnect...")
-                break
-
-        self.__sub(action = "all")
-
-    def __is_connection_alive(self) -> bool:
-        alive = False
-        status = f"Socket is null : {self._sock is None}, socket file stream is null : {self._socket_fs is None}, "
-        if (self._sock is not None) and (self._socket_fs is not None) :
-            LOGGER.debug(status + f"Socket is closed : {self._sock._closed}, socket file stream is closed : {self._socket_fs.closed}")
-            if (not self._sock._closed) and (not self._socket_fs.closed):
-                alive = True
-        return alive
-
-    def __do_connection(self):
-        ''' Create connection; if it fails inititate retry logic '''
-
-        try :
-            self.__create_connection()
-        except OSError:
-            self.__retry_connection()
-
-    def __create_connection(self):
-        # New code TCP
-        self._sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self._sock.settimeout(100)
-
-        self._sock.connect((self.__host, self.__port)) # raises OSError
-        self._sock.setblocking(True)
-
-        self._socket_fs = self._sock.makefile('rw')
-        LOGGER.info("Connection established with subscriber.")
-
-    def __retry_connection(self):
-        times = 17000  # ~17000 for ~24 hours with delay of 5 seconds
-        initalDelay = 1 # seconds
-        maxDelay = 5 # seconds
-        delayFactor = 2.0
-
-        currentDelay = initalDelay
-        for currentTry in range(times, 0, -1):
-            try :
-                self.__create_connection()
-            except OSError as e:
-                LOGGER.error(f"Error : {e}. Failed to establish connection with the streaming socket. Retrying socket connection... Max tries left {currentTry}")
-                sleep(currentDelay)
-                currentDelay = currentDelay*delayFactor if currentDelay*delayFactor < maxDelay else maxDelay
-            else:
-                break
-        else:
-            #last attempt
-            try :
-                self.__create_connection()
-            except OSError as e:
-                LOGGER.error(f"Failed to connect with streaming socket after {times} unsuccessful retry attempts. Error : {e}")
-                self._sock.close()
-                raise e
+from cgitb import Hook
+import json
+import logging
+import socket
+from threading import Thread
+from time import sleep
+from typing import Any, Callable
+
+from constants.streaming_constants import StreamingConstants
+
+LOGGER = logging.getLogger(__name__)
+
+class Feed:
+
+    def __init__(self, confObj):
+        self.__conf = confObj
+
+        AppIdKey = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhcHAiOjAsImZmIjoiVyIsImJkIjoid2ViLXBjIiwibmJmIjoxNjg0NTAwMDU0LCJzcmMiOiJlbXRtdyIsImF2IjoiMi4wLjIiLCJhcHBpZCI6ImM0YTFmYjE1Yjk2Y2E5OGRiOWVkOTVkNmFkZmJlOWM2IiwiaXNzIjoiZW10IiwiZXhwIjoxNjg0NTIxMDAwLCJpYXQiOjE2ODQ1MDAzNTR9.XuH-LuW3STn15EjZNmh31ZqNUsl98r_8aIJfmJ_CapE"
+        Host="ncst.nuvamawealth.com"
+        Port=9443
+
+        self._appID = AppIdKey
+        self.__host = Host
+        self.__port = Port
+
+        if self.__conf:
+            if self.__conf['GLOBAL'].get('AppIdKey'):
+                self._appID = self.__conf['GLOBAL'].get('AppIdKey')
+            if self.__conf['STREAM'].get('HOST'):
+                self.__host = self.__conf['STREAM'].get('HOST')
+            if self.__conf['STREAM'].get('PORT'):
+                self.__port = int(self.__conf['STREAM'].get('PORT'))
+        self._sock = None
+        self._socket_fs = None
+        self.__requestsList = {}
+
+        t = Thread(target=self.__do_connection)
+        t.start()
+
+    def _subscribe(self, request : str, callback : Callable[[str], Any], requestCode : StreamingConstants):
+        self.__requestsList[requestCode] = {'request' : request, 'callback' : callback}
+        self.__sub(requestCode)
+
+    def _unsubscribe(self, request : str, requestCode : StreamingConstants):
+        if self.__is_connection_alive():
+            self.__send_stream_request(request)
+        else :
+            self.__do_connection()
+            self.__send_stream_request(request)
+        self.__requestsList.pop(requestCode, "Key not found")
+
+
+    def __sub(self, action):
+        if self.__is_connection_alive():
+            if action == 'all':
+                for req_code in self.__requestsList.keys():
+                    self.__start_streaming(self.__requestsList[req_code]['request'])
+                    sleep(0.1)
+            elif type(action) is StreamingConstants:
+                self.__start_streaming(self.__requestsList[action]['request'])
+        else:
+            self.__do_connection()
+            self.__sub(action)
+
+    def __start_streaming(self, sendRequest : str):
+        self.__send_stream_request(sendRequest)
+        t_read = Thread(target = self.__read_stream_data)
+        t_read.start()
+
+    def __send_stream_request(self, request : str):
+        self._socket_fs.writelines(request)
+        self._socket_fs.flush()
+
+    def __read_stream_data(self):
+        while True:
+            resp = self._socket_fs.readline()
+
+            if resp:
+                LOGGER.debug(f"Response recevied : {resp}")
+                try:
+                    resp_dict = json.loads(resp)
+
+                    if resp_dict['response']["streaming_type"] == "quote3":
+                        callback = self.__requestsList[StreamingConstants.QUOTE_SREAM_REQ_CODE]['callback']
+                    elif resp_dict['response']["streaming_type"] == "orderFiler":
+                        callback = self.__requestsList[StreamingConstants.ORDER_STREAM_REQ_CODE]['callback']
+                    elif resp_dict['response']["streaming_type"] == "news":
+                        callback = self.__requestsList[StreamingConstants.LIVENEWS_STREAM_REQ_CODE]['callback']
+
+                    callback(resp)
+
+                except json.JSONDecodeError:
+                    pass
+
+            else:
+                LOGGER.error("Response Blank. Socket Connection seems to be closed. Trying to reconnect...")
+                break
+
+        self.__sub(action = "all")
+
+    def __is_connection_alive(self) -> bool:
+        alive = False
+        status = f"Socket is null : {self._sock is None}, socket file stream is null : {self._socket_fs is None}, "
+        if (self._sock is not None) and (self._socket_fs is not None) :
+            LOGGER.debug(status + f"Socket is closed : {self._sock._closed}, socket file stream is closed : {self._socket_fs.closed}")
+            if (not self._sock._closed) and (not self._socket_fs.closed):
+                alive = True
+        return alive
+
+    def __do_connection(self):
+        ''' Create connection; if it fails inititate retry logic '''
+
+        try :
+            self.__create_connection()
+        except OSError:
+            self.__retry_connection()
+
+    def __create_connection(self):
+        # New code TCP
+        self._sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self._sock.settimeout(100)
+
+        self._sock.connect((self.__host, self.__port)) # raises OSError
+        self._sock.setblocking(True)
+
+        self._socket_fs = self._sock.makefile('rw')
+        LOGGER.info("Connection established with subscriber.")
+
+    def __retry_connection(self):
+        times = 17000  # ~17000 for ~24 hours with delay of 5 seconds
+        initalDelay = 1 # seconds
+        maxDelay = 5 # seconds
+        delayFactor = 2.0
+
+        currentDelay = initalDelay
+        for currentTry in range(times, 0, -1):
+            try :
+                self.__create_connection()
+            except OSError as e:
+                LOGGER.error(f"Error : {e}. Failed to establish connection with the streaming socket. Retrying socket connection... Max tries left {currentTry}")
+                sleep(currentDelay)
+                currentDelay = currentDelay*delayFactor if currentDelay*delayFactor < maxDelay else maxDelay
+            else:
+                break
+        else:
+            #last attempt
+            try :
+                self.__create_connection()
+            except OSError as e:
+                LOGGER.error(f"Failed to connect with streaming socket after {times} unsuccessful retry attempts. Error : {e}")
+                self._sock.close()
+                raise e
```

### Comparing `APIConnect-2.0.1.post1/feed/livenews_feed.py` & `APIConnect-2.0.2/feed/orders_feed.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,59 @@
-import json
-import logging
-from typing import Any, Callable
-from APIConnect.validator import Validator
-from constants.streaming_constants import StreamingConstants
-from feed.feed import Feed
-
-LOGGER = logging.getLogger(__name__)
-
-
-class LiveNewsFeed():
-
-    def __init__(self, feedObj : Feed ) -> None:
-        self.__feed_obj = feedObj
-
-    @Validator.isRequired(["callBack"])
-    def subscribeLiveNewsFeed(self, callBack: Callable[[str], Any]) -> None:
-        livenews_req = self.__create_livenews_request()
-        LOGGER.debug(f"Subscribing live news feed with request : {livenews_req}")
-
-        self.__feed_obj._subscribe(livenews_req, callBack, StreamingConstants.LIVENEWS_STREAM_REQ_CODE)
-
-    def unsubscribeLiveNewsFeed(self) -> None:
-        unsub_news_req = self.__create_livenews_request(subscribe=False)
-        LOGGER.debug(
-            f"Unsubscribing live news feed with request : {unsub_news_req}")
-        self.__feed_obj._unsubscribe(unsub_news_req, StreamingConstants.LIVENEWS_STREAM_REQ_CODE)
-
-    def __create_livenews_request(self, subscribe: bool = True) -> str:
-
-        if subscribe:
-            req_type = "subscribe"
-        else:
-            req_type = "unsubscribe"
-
-        req = {
-            "request":
-                {
-                    "streaming_type": "news",
-                    "formFactor": "P",
-                    "appID": self.__feed_obj._appID,
-                    "response_format": "json",
-                    "request_type": req_type,
-                },
-            "echo": {}
-        }
-        return json.dumps(req) + "\n"
+import json
+import logging
+from typing import Any, Callable
+from APIConnect.validator import Validator
+from constants.streaming_constants import StreamingConstants
+from feed.feed import Feed
+
+LOGGER = logging.getLogger(__name__)
+
+
+class OrdersFeed():
+
+
+    def __init__(self, feedObj : Feed, acc_id : str, user_id : str) -> None:
+        self.acc_id = acc_id
+        self.user_id = user_id
+        self.__feed_obj = feedObj
+
+    @Validator.isRequired(["callBack"])
+    def subscribeOrdersFeed(self, callBack: Callable[[str], Any]) -> None:
+        order_req = self.__create_order_request()
+        LOGGER.debug(f"Subscribing orders feed with request: {order_req}")
+        # self.__feed_obj._socket_fs.writelines(order_req)
+        # self.__feed_obj._socket_fs.flush()
+
+        self.__feed_obj._subscribe(order_req, callBack, StreamingConstants.ORDER_STREAM_REQ_CODE)
+
+    def unsubscribeOrdersFeed(self) -> None:
+        unsub_order_req = self.__create_order_request(subscribe=False)
+        LOGGER.debug(
+            f"Unsubscribing orders feed with request: {unsub_order_req}")
+        self.__feed_obj._unsubscribe(unsub_order_req, StreamingConstants.ORDER_STREAM_REQ_CODE)
+
+    def __create_order_request(self, subscribe: bool = True) -> str:
+
+        if subscribe:
+            req_type = "subscribe"
+        else:
+            req_type = "unsubscribe"
+
+        req = {
+            "request":
+                {
+                    "streaming_type": "orderFiler",
+                    "data":
+                        {
+                            "accType": "EQ",
+                            "userID": self.user_id,
+                            "accID": self.acc_id,
+                            "responseType": ["ORDER_UPDATE", "TRADE_UPDATE"]
+                        },
+                    "formFactor": "P",
+                    "appID": self.__feed_obj._appID,
+                    "response_format": "json",
+                    "request_type": req_type,
+                },
+            "echo": {}
+        }
+        return json.dumps(req) + "\n"
```

### Comparing `APIConnect-2.0.1.post1/feed/quotes_feed.py` & `APIConnect-2.0.2/feed/quotes_feed.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import json
-import logging
-from typing import Any, Callable, List
-from APIConnect.validator import Validator
-from constants.streaming_constants import StreamingConstants
-from feed.feed import Feed
-
-LOGGER = logging.getLogger(__name__)
-
-
-class QuotesFeed():
-
-    @Validator.ValidateInputDataTypes
-    def __init__(self, feedObj : Feed) -> None:
-        self.__feed_obj = feedObj
-
-    @Validator.isRequired(["symbols", "callBack"])
-    def subscribeQuotesFeed(self, symbols: List[str], callBack: Callable[[str], Any]) -> None:
-        quote = self.__create_quote_request(symbols)
-        LOGGER.debug("Subscribing quote feed with request: %s", quote)
-
-        self.__feed_obj._subscribe(quote, callBack, StreamingConstants.QUOTE_SREAM_REQ_CODE)
-
-    @Validator.isRequired(["symbols"])
-    def unsubscribeQuotesFeed(self) -> None:
-        '''
-
-         This method will unsubscribe from the streamer. After successful invokation, this will stop the streamer packets of the symbols subscribed.
-
-        '''
-        unsub_quote = self.__create_quote_request(subscribe = False)
-        LOGGER.debug("Unsubscribing quote feed with request: %s", unsub_quote)
-        self.__feed_obj._unsubscribe(unsub_quote, StreamingConstants.QUOTE_SREAM_REQ_CODE)
-
-    def __create_quote_request(self, symbols = [], subscribe: bool = True) -> str:
-
-        symset = []
-        for syms in symbols:
-            symset.append({"symbol": syms})
-        if subscribe:
-            request_type = "subscribe"
-        else:
-            request_type = "unsubscribe"
-        req = {
-            "request":
-                {
-                    "streaming_type": "quote3",
-                    "data":
-                        {
-                            "accType": "EQ",
-                            "symbols": symset
-                        },
-                    "formFactor": "P",
-                    "appID": self.__feed_obj._appID,
-                    "response_format": "json",
-                    "request_type": request_type
-                },
-            "echo": {}
-        }
-        return json.dumps(req) + "\n"
+import json
+import logging
+from typing import Any, Callable, List
+from APIConnect.validator import Validator
+from constants.streaming_constants import StreamingConstants
+from feed.feed import Feed
+
+LOGGER = logging.getLogger(__name__)
+
+
+class QuotesFeed():
+
+    @Validator.ValidateInputDataTypes
+    def __init__(self, feedObj : Feed) -> None:
+        self.__feed_obj = feedObj
+
+    @Validator.isRequired(["symbols", "callBack"])
+    def subscribeQuotesFeed(self, symbols: List[str], callBack: Callable[[str], Any]) -> None:
+        quote = self.__create_quote_request(symbols)
+        LOGGER.debug("Subscribing quote feed with request: %s", quote)
+
+        self.__feed_obj._subscribe(quote, callBack, StreamingConstants.QUOTE_SREAM_REQ_CODE)
+
+    @Validator.isRequired(["symbols"])
+    def unsubscribeQuotesFeed(self) -> None:
+        '''
+
+         This method will unsubscribe from the streamer. After successful invokation, this will stop the streamer packets of the symbols subscribed.
+
+        '''
+        unsub_quote = self.__create_quote_request(subscribe = False)
+        LOGGER.debug("Unsubscribing quote feed with request: %s", unsub_quote)
+        self.__feed_obj._unsubscribe(unsub_quote, StreamingConstants.QUOTE_SREAM_REQ_CODE)
+
+    def __create_quote_request(self, symbols = [], subscribe: bool = True) -> str:
+
+        symset = []
+        for syms in symbols:
+            symset.append({"symbol": syms})
+        if subscribe:
+            request_type = "subscribe"
+        else:
+            request_type = "unsubscribe"
+        req = {
+            "request":
+                {
+                    "streaming_type": "quote3",
+                    "data":
+                        {
+                            "accType": "EQ",
+                            "symbols": symset
+                        },
+                    "formFactor": "P",
+                    "appID": self.__feed_obj._appID,
+                    "response_format": "json",
+                    "request_type": request_type
+                },
+            "echo": {}
+        }
+        return json.dumps(req) + "\n"
```

### Comparing `APIConnect-2.0.1.post1/resources/watchlist_resource.py` & `APIConnect-2.0.2/resources/watchlist_resource.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import json
-import logging
-
-LOGGER = logging.getLogger(__name__)
-
-class WatchlistResource :
-    def __init__(self, response : str) -> None:
-
-        LOGGER.debug(f"{self.__class__.__name__} object is being created.")
-
-        self._response = response
-        self.__response_dict = json.loads(self._response)
-        self.__messageID = self.__response_dict['msgID']
-        self.__serverTime = self.__response_dict['srvTm']
-        self.__data = self.__response_dict['data']
-
-    def _getWatchlistFormatted(self) -> 'WatchlistResource' :
-        LOGGER.debug("inside _getWatchlistFormatted method")
-
-        formatted_resp_dict = {
-                            'data' : self.__data,
-                            'msgID' : self.__messageID,
-                            'srvTm' : self.__serverTime
-                            }
-        self._response = json.dumps(formatted_resp_dict)
+import json
+import logging
+
+LOGGER = logging.getLogger(__name__)
+
+class WatchlistResource :
+    def __init__(self, response : str) -> None:
+
+        LOGGER.debug(f"{self.__class__.__name__} object is being created.")
+
+        self._response = response
+        self.__response_dict = json.loads(self._response)
+        self.__messageID = self.__response_dict['msgID']
+        self.__serverTime = self.__response_dict['srvTm']
+        self.__data = self.__response_dict['data']
+
+    def _getWatchlistFormatted(self) -> 'WatchlistResource' :
+        LOGGER.debug("inside _getWatchlistFormatted method")
+
+        formatted_resp_dict = {
+                            'data' : self.__data,
+                            'msgID' : self.__messageID,
+                            'srvTm' : self.__serverTime
+                            }
+        self._response = json.dumps(formatted_resp_dict)
         return self
```

### Comparing `APIConnect-2.0.1.post1/services/live_news_service.py` & `APIConnect-2.0.2/services/live_news_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,207 +1,208 @@
-import json
-import logging
-from typing import Tuple, Union
-from APIConnect.validator import Validator
-from constants.results_stocks_news_category import ResultsAndStocksNewsCategoryEnum
-from exceptions.api_exception import APIError
-from exceptions.validation_exception import ValidationException
-from resources.live_news_resource import LiveNewsResource
-
-LOGGER = logging.getLogger(__name__)
-
-class LiveNewsService():
-    def __init__(self, routerObj, httpObj, fileName) -> None:
-        LOGGER.debug("LiveNewsService object is being created.")
-
-        self.__routerObj = routerObj
-        self.__http = httpObj
-        self.__fileName = fileName
-        self.__excludeCategories = ['Results', 'Stocks in News', 'My Holdings']
-        self.__allCategoriesDataDict = {}
-        self.__validCategoriesList = []
-
-    def _getNewsCategories(self) -> str :
-        LOGGER.debug("inside _getNewsCategories method")
-        all_categories_resp = self.__getAllNewsCategories()
-        if all_categories_resp != "":
-            filtered_response = LiveNewsResource(all_categories_resp)._getCategoriesFormatted()._filterCategories(self.__excludeCategories)._response
-            self.__validCategoriesList = json.loads(filtered_response)['data']['categories']
-            return filtered_response
-        else:
-            return all_categories_resp
-
-    @Validator.isRequired(['category'])
-    def _getGeneralNews(self, category : str, searchText : str = None, pageNumber : int = None) -> str :
-        LOGGER.debug("inside _getGeneralNews method")
-        response = ""
-
-        self._getNewsCategories()
-
-        if self.__validCategoriesList:
-            specific_cat_dict, special = self.__getSpecificCategoryData(category)
-
-            if specific_cat_dict :
-                request_body = {
-                    "exclCategory": [] if special else specific_cat_dict["exc"],
-                    "inclCategory": [specific_cat_dict["cat"]] if special else specific_cat_dict["inc"],
-                    "validRequest": None if special else specific_cat_dict["lgrq"],
-                    "page": pageNumber,
-                    "group": specific_cat_dict['uiTyp'],
-                    "searchText": searchText
-                }
-                response = self.__getGeneralNewsAPI(request_body)
-                if response != '""':
-                    response = LiveNewsResource(response, specific_cat_dict['uiTyp'])._getNewsFormatted()._response
-        return response
-
-    def _getHoldingsNews(self, category : Union[str, list] = None, searchText : str = None, pageNumber : int = None) -> str :
-        LOGGER.debug("inside _getHoldingsNews method")
-        response = ""
-        category_list = []
-        if category:
-            category_list.extend(category) if type(category) is list else category_list.append(category)
-
-        self._getNewsCategories()
-        if self.__validCategoriesList:
-            holdings_cat_data, _ = self.__getSpecificCategoryData("My Holdings", True)
-            request_body = {
-                "exclCategory": holdings_cat_data["exc"],
-                "inclCategory": holdings_cat_data["inc"],
-                "validRequest": holdings_cat_data["lgrq"],
-                "group": holdings_cat_data["uiTyp"],
-                "page": pageNumber,
-                "searchText": searchText
-            }
-
-            response = self.__getHoldingsNewsAPI(request_body)
-
-            if response != '""':
-                response = LiveNewsResource(response, holdings_cat_data["uiTyp"])._getNewsFormatted()._response
-
-                if category and category != "All" : # if category is All, no filtering required
-
-                    if sorted(category) == sorted([e.value for e in ResultsAndStocksNewsCategoryEnum]):
-                        self.__validCategoriesList = [e.value for e in ResultsAndStocksNewsCategoryEnum]
-
-                    filter_categories = []
-                    for cat in category_list :
-                        cat_dict, special = self.__getSpecificCategoryData(cat)
-                        filter_categories.append(cat_dict["cat"]) if special else filter_categories.extend(cat_dict["inc"])
-
-                    response = LiveNewsResource(response, category_dp_name=category)._filterCategories(filter_categories, exclude=False)._response
-
-        return response
-
-    def _getResultsAndStocksNews(self, searchText : str = None, pageNumber : int = None) -> str :
-        LOGGER.debug("inside _getResultsAndStocksNews method")
-        response = ""
-
-        request_body = {
-            "exclCategory": [],
-            "inclCategory": ["Result", "STOCK_IN_NEWS"],
-            "validRequest":  False,
-            "page": pageNumber,
-            "group": "G",
-            "searchText": searchText
-        }
-        response = self.__getGeneralNewsAPI(request_body)
-        if response != '""':
-            response = LiveNewsResource(response, "G")._getNewsFormatted()._response
-        return response
-
-
-    def __getSpecificCategoryData(self, category : str, holdings : bool = False) -> Tuple[dict, bool]:
-        LOGGER.debug("inside __getSpecificCategoryData method")
-        cat_data = {}
-        special = False
-        if self.__allCategoriesDataDict :
-            #TODO: test this
-            if holdings or category in self.__validCategoriesList :
-                for key, value in self.__allCategoriesDataDict['data'].items():
-                    if type(value) is list:
-                        for cat_dict in value:
-                            if 'dpNm' in cat_dict.keys() and cat_dict['dpNm'] == category:
-                                if key == "ctLst":
-                                   special = True
-                                cat_data = cat_dict
-                                break
-            else :
-                raise ValidationException(f"'{category}' is not a valid category. Please call getNewsCategories function to retrieve all valid categories.")
-
-        return cat_data, special
-
-    def __getAllNewsCategories(self) -> str:
-        '''method to either read all categories from user session file or get all categories from categories API'''
-        LOGGER.debug("inside __getAllNewsCategories method")
-
-        try:
-            with open(self.__fileName, 'r+') as fs:
-                read = fs.read()
-                user_data_dict = json.loads(read)
-                # if categories saved in data_ApiKey.txt file
-                if 'newsCategories' in user_data_dict.keys():
-                    LOGGER.debug(f"Reading categories response from user data file." )
-                    self.__allCategoriesDataDict = user_data_dict['newsCategories']
-                    newsCategoriesResponse = json.dumps(self.__allCategoriesDataDict)
-                # if categories not saved in file, call api and save response in data_ApiKey.txt
-                else :
-                    newsCategoriesResponse = self.__getAllNewsCategoriesAPI()
-                    if newsCategoriesResponse != "":
-                        self.__allCategoriesDataDict = json.loads(newsCategoriesResponse)
-                        user_data_dict['newsCategories'] = self.__allCategoriesDataDict
-                        # deleting contents of data_ApiKey.txt and writing categories-appended-data
-                        fs.seek(0)
-                        fs.truncate()
-                        fs.write(json.dumps(user_data_dict))
-                        LOGGER.debug("Categories response saved to user data file.")
-            return newsCategoriesResponse
-        except FileNotFoundError:
-            LOGGER.error(f"Session file {self.__fileName} not found. Kindly login again.")
-            raise APIError("Session file not found. Kindly login again.")
-        except OSError as e:
-            LOGGER.error(f"Error in reading/writing {self.__fileName} : {e}")
-            raise e
-
-    def __getAllNewsCategoriesAPI(self) -> str:
-
-        LOGGER.debug("inside __getAllNewsCategoriesAPI method")
-
-        url = self.__routerObj._LiveNewsCategoriesURL()
-        reply = self.__http._GetMethod(url)
-        LOGGER.debug(f"Response received: {reply}")
-
-        return json.dumps(reply)
-
-    def __getGeneralNewsAPI(self, request_body) -> str:
-
-        LOGGER.debug("inside __getGeneralNewsAPI method")
-
-        url = self.__routerObj._GeneralNewsURL()
-        body = json.dumps(request_body)
-
-        LOGGER.debug("__getGeneralNewsAPI method is called with data: %s", body)
-        reply = self.__http._PostMethod(url, body)
-        LOGGER.debug(f"Response received: {reply}")
-
-        return json.dumps(reply)
-
-    def __getHoldingsNewsAPI(self, request_body ) -> str:
-
-        LOGGER.debug("inside __getHoldingsNewsAPI method")
-        url = self.__routerObj._HoldingsNewsURL()
-        body = json.dumps(request_body)
-
-        LOGGER.debug("__getHoldingsNewsAPI method is called with data: %s", body)
-        reply = self.__http._PostMethod(url, body)
-        LOGGER.debug(f"Response received: {reply}")
-
-        return json.dumps(reply)
-
-    def _getLatestCorpActionsAPI(self, symbol : str) -> str:
-
-        LOGGER.debug("inside __getLatestCorpActionsAPI method")
-        url = self.__routerObj._LatestCorpActionsURL().format(symbol = symbol)
-        reply = self.__http._GetMethod(url)
-        LOGGER.debug(f"Response received: {reply}")
-
+import json
+import logging
+from typing import Tuple, Union
+from APIConnect.http import Http
+from APIConnect.validator import Validator
+from constants.results_stocks_news_category import ResultsAndStocksNewsCategoryEnum
+from constants.router import Router
+from exceptions.api_exception import APIError
+from exceptions.validation_exception import ValidationException
+from resources.live_news_resource import LiveNewsResource
+
+LOGGER = logging.getLogger(__name__)
+
+class LiveNewsService():
+    def __init__(self, routerObj, httpObj, fileName) -> None:
+        LOGGER.debug("LiveNewsService object is being created.")
+
+        self.__routerObj : Router = routerObj
+        self.__http : Http = httpObj
+        self.__fileName = fileName
+        self.__excludeCategories = ['Results', 'Stocks in News', 'My Holdings']
+        self.__allCategoriesDataDict = {}
+        self.__validCategoriesList = []
+
+    def _getNewsCategories(self) -> str :
+        LOGGER.debug("inside _getNewsCategories method")
+        all_categories_resp = self.__getAllNewsCategories()
+        if all_categories_resp != "":
+            filtered_response = LiveNewsResource(all_categories_resp)._getCategoriesFormatted()._filterCategories(self.__excludeCategories)._response
+            self.__validCategoriesList = json.loads(filtered_response)['data']['categories']
+            return filtered_response
+        else:
+            return all_categories_resp
+
+    @Validator.isRequired(['category'])
+    def _getGeneralNews(self, category : str, searchText : str = None, pageNumber : int = None) -> str :
+        LOGGER.debug("inside _getGeneralNews method")
+        response = ""
+
+        self._getNewsCategories()
+
+        if self.__validCategoriesList:
+            specific_cat_dict, special = self.__getSpecificCategoryData(category)
+
+            if specific_cat_dict :
+                request_body = {
+                    "exclCategory": [] if special else specific_cat_dict["exc"],
+                    "inclCategory": [specific_cat_dict["cat"]] if special else specific_cat_dict["inc"],
+                    "validRequest": None if special else specific_cat_dict["lgrq"],
+                    "page": pageNumber,
+                    "group": specific_cat_dict['uiTyp'],
+                    "searchText": searchText
+                }
+                response = self.__getGeneralNewsAPI(request_body)
+                if response != '""':
+                    response = LiveNewsResource(response, specific_cat_dict['uiTyp'])._getNewsFormatted()._response
+        return response
+
+    def _getHoldingsNews(self, category : Union[str, list] = None, searchText : str = None, pageNumber : int = None) -> str :
+        LOGGER.debug("inside _getHoldingsNews method")
+        response = ""
+        category_list = []
+        if category:
+            category_list.extend(category) if type(category) is list else category_list.append(category)
+
+        self._getNewsCategories()
+        if self.__validCategoriesList:
+            holdings_cat_data, _ = self.__getSpecificCategoryData("My Holdings", True)
+            request_body = {
+                "exclCategory": holdings_cat_data["exc"],
+                "inclCategory": holdings_cat_data["inc"],
+                "validRequest": holdings_cat_data["lgrq"],
+                "group": holdings_cat_data["uiTyp"],
+                "page": pageNumber,
+                "searchText": searchText
+            }
+
+            response = self.__getHoldingsNewsAPI(request_body)
+
+            if response != '""':
+                response = LiveNewsResource(response, holdings_cat_data["uiTyp"])._getNewsFormatted()._response
+
+                if category and category != "All" : # if category is All, no filtering required
+
+                    if sorted(category) == sorted([e.value for e in ResultsAndStocksNewsCategoryEnum]):
+                        self.__validCategoriesList = [e.value for e in ResultsAndStocksNewsCategoryEnum]
+
+                    filter_categories = []
+                    for cat in category_list :
+                        cat_dict, special = self.__getSpecificCategoryData(cat)
+                        filter_categories.append(cat_dict["cat"]) if special else filter_categories.extend(cat_dict["inc"])
+
+                    response = LiveNewsResource(response, category_dp_name=category)._filterCategories(filter_categories, exclude=False)._response
+
+        return response
+
+    def _getResultsAndStocksNews(self, searchText : str = None, pageNumber : int = None) -> str :
+        LOGGER.debug("inside _getResultsAndStocksNews method")
+        response = ""
+
+        request_body = {
+            "exclCategory": [],
+            "inclCategory": ["Result", "STOCK_IN_NEWS"],
+            "validRequest":  False,
+            "page": pageNumber,
+            "group": "G",
+            "searchText": searchText
+        }
+        response = self.__getGeneralNewsAPI(request_body)
+        if response != '""':
+            response = LiveNewsResource(response, "G")._getNewsFormatted()._response
+        return response
+
+
+    def __getSpecificCategoryData(self, category : str, holdings : bool = False) -> Tuple[dict, bool]:
+        LOGGER.debug("inside __getSpecificCategoryData method")
+        cat_data = {}
+        special = False
+        if self.__allCategoriesDataDict :
+            if holdings or category in self.__validCategoriesList :
+                for key, value in self.__allCategoriesDataDict['data'].items():
+                    if type(value) is list:
+                        for cat_dict in value:
+                            if 'dpNm' in cat_dict.keys() and cat_dict['dpNm'] == category:
+                                if key == "ctLst":
+                                    special = True
+                                cat_data = cat_dict
+                                break
+            else :
+                raise ValidationException(f"'{category}' is not a valid category. Please call getNewsCategories function to retrieve all valid categories.")
+
+        return cat_data, special
+
+    def __getAllNewsCategories(self) -> str:
+        '''method to either read all categories from user session file or get all categories from categories API'''
+        LOGGER.debug("inside __getAllNewsCategories method")
+
+        try:
+            with open(self.__fileName, 'r+') as fs:
+                read = fs.read()
+                user_data_dict = json.loads(read)
+                # if categories saved in data_ApiKey.txt file
+                if 'newsCategories' in user_data_dict.keys():
+                    LOGGER.debug(f"Reading categories response from user data file." )
+                    self.__allCategoriesDataDict = user_data_dict['newsCategories']
+                    newsCategoriesResponse = json.dumps(self.__allCategoriesDataDict)
+                # if categories not saved in file, call api and save response in data_ApiKey.txt
+                else :
+                    newsCategoriesResponse = self.__getAllNewsCategoriesAPI()
+                    if newsCategoriesResponse != "":
+                        self.__allCategoriesDataDict = json.loads(newsCategoriesResponse)
+                        user_data_dict['newsCategories'] = self.__allCategoriesDataDict
+                        # deleting contents of data_ApiKey.txt and writing categories-appended-data
+                        fs.seek(0)
+                        fs.truncate()
+                        fs.write(json.dumps(user_data_dict))
+                        LOGGER.debug("Categories response saved to user data file.")
+            return newsCategoriesResponse
+        except FileNotFoundError:
+            LOGGER.error(f"Session file {self.__fileName} not found. Kindly login again.")
+            raise APIError("Session file not found. Kindly login again.")
+        except OSError as e:
+            LOGGER.error(f"Error in reading/writing {self.__fileName} : {e}")
+            raise e
+
+    def __getAllNewsCategoriesAPI(self) -> str:
+
+        LOGGER.debug("inside __getAllNewsCategoriesAPI method")
+
+        url = self.__routerObj._LiveNewsCategoriesURL()
+        reply = self.__http._GetMethod(url)
+        LOGGER.debug(f"Response received: {reply}")
+
+        return json.dumps(reply)
+
+    def __getGeneralNewsAPI(self, request_body) -> str:
+
+        LOGGER.debug("inside __getGeneralNewsAPI method")
+
+        url = self.__routerObj._GeneralNewsURL()
+        body = json.dumps(request_body)
+
+        LOGGER.debug("__getGeneralNewsAPI method is called with data: %s", body)
+        reply = self.__http._PostMethod(url, body)
+        LOGGER.debug(f"Response received: {reply}")
+
+        return json.dumps(reply)
+
+    def __getHoldingsNewsAPI(self, request_body ) -> str:
+
+        LOGGER.debug("inside __getHoldingsNewsAPI method")
+        url = self.__routerObj._HoldingsNewsURL()
+        body = json.dumps(request_body)
+
+        LOGGER.debug("__getHoldingsNewsAPI method is called with data: %s", body)
+        reply = self.__http._PostMethod(url, body)
+        LOGGER.debug(f"Response received: {reply}")
+
+        return json.dumps(reply)
+
+    def _getLatestCorpActionsAPI(self, symbol : str) -> str:
+
+        LOGGER.debug("inside __getLatestCorpActionsAPI method")
+        url = self.__routerObj._LatestCorpActionsURL().format(symbol = symbol)
+        reply = self.__http._GetMethod(url)
+        LOGGER.debug(f"Response received: {reply}")
+
         return json.dumps(reply)
```

### Comparing `APIConnect-2.0.1.post1/services/watchlist_service.py` & `APIConnect-2.0.2/services/watchlist_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,258 +1,258 @@
-import json
-import logging
-import sys
-import time
-from typing import List
-from APIConnect.api_utils import ApiUtils
-from APIConnect.http import Http
-from constants.router import Router
-from resources.watchlist_resource import WatchlistResource
-
-LOGGER = logging.getLogger(__name__)
-
-class WatchlistService:
-    def __init__(self, routerObj, httpObj, constantsObj) -> None:
-        LOGGER.debug("WatchlistService object is being created.")
-
-        self.__routerObj : Router = routerObj
-        self.__http : Http = httpObj
-        self.__constants : ApiUtils = constantsObj
-        self.__accId = None
-        self.__accType = None
-        self.__profileId = None
-
-    def _getWatchlistGroups(self) -> str :
-        LOGGER.debug("inside _getWatchlistGroups method")
-
-        self.__getUserAccData()
-
-        url = self.__routerObj._WatchlistBaseGroupsURL()
-        queryParams = {"accId" : self.__accId, "accTyp" : self.__accType}
-
-        response = self.__getGroupsWatchlistAPI(url, queryParams)
-        if response :
-            formatted_resp = WatchlistResource(response)._getWatchlistFormatted()._response
-            return formatted_resp
-        return response
-
-    def _getScripsOfGroup(self, GroupName : str) -> str :
-        LOGGER.debug("inside _getScripsOfGroup method")
-
-        self.__getUserAccData()
-
-        url = self.__routerObj._WatchlistGetScripsURL()
-        queryParams = {"accId" : self.__accId, "accTyp" : self.__accType, "prfId" : self.__profileId, "grpNm" : GroupName}
-
-        response = self.__getScripsOfGroupAPI(url, queryParams)
-        if response :
-            formatted_resp = WatchlistResource(response)._getWatchlistFormatted()._response
-            return formatted_resp
-        return response
-
-    def _createGroup(self, GroupName : str, Symbols : List[str]) -> str :
-        LOGGER.debug("inside _createGroup method")
-
-        self.__getUserAccData()
-
-        url = self.__routerObj._WatchlistGroupNameURL().format(groupName = GroupName)
-        request_body = {
-                        "accId": self.__accId,
-                        "accTyp": self.__accType,
-                        "prfId": self.__profileId,
-                        "grpNm": GroupName,
-                        "symLst": Symbols
-                        }
-        LOGGER.debug(f"_createGroup method is called with data : {request_body}")
-        response = self.__createGroupAPI(url, json.dumps(request_body))
-        if response :
-            formatted_resp = WatchlistResource(response)._getWatchlistFormatted()._response
-            return formatted_resp
-        return response
-
-    def _addSymbols(self, GroupName : str, Symbols : List[str]) -> str :
-        LOGGER.debug("inside _addSymbol method")
-
-        self.__getUserAccData()
-        currentUnixTimeStamp = int(time.time()*1000)
-
-        url = self.__routerObj._WatchlistGroupNameURL().format(groupName = GroupName)
-        request_body = {
-                        "accId": self.__accId,
-                        "accTyp": self.__accType,
-                        "act": "add",
-                        "grpNm": GroupName,
-                        "symLst": Symbols,
-                        "updatedOn" : currentUnixTimeStamp
-                        }
-        LOGGER.debug(f"_addSymbol method is called with data : {request_body}")
-        response = self.__addSymbolAPI(url, json.dumps(request_body))
-        if response :
-            formatted_resp = WatchlistResource(response)._getWatchlistFormatted()._response
-            return formatted_resp
-        return response
-
-    def _deleteSymbols(self, GroupName : str, Symbols : List[str]) -> str :
-        LOGGER.debug("inside _deleteSymbols method")
-
-        self.__getUserAccData()
-        currentUnixTimeStamp = int(time.time()*1000)
-
-        url = self.__routerObj._WatchlistGroupNameURL().format(groupName = GroupName)
-        request_body = {
-                        "accId": self.__accId,
-                        "accTyp": self.__accType,
-                        "act": "del",
-                        "grpNm": GroupName,
-                        "symLst": Symbols,
-                        "updatedOn" : currentUnixTimeStamp
-                        }
-        LOGGER.debug(f"_deleteSymbols method is called with data : {request_body}")
-        response = self.__deleteSymbolAPI(url, json.dumps(request_body))
-        if response :
-            formatted_resp = WatchlistResource(response)._getWatchlistFormatted()._response
-            return formatted_resp
-        return response
-
-    def _deleteGroups(self, GroupNames : List[str]) -> str :
-        LOGGER.debug("inside _deleteGroups method")
-
-        self.__getUserAccData()
-
-        url = self.__routerObj._WatchlistBaseGroupsURL()
-        request_body = {
-                        "accId": self.__accId,
-                        "accTyp": self.__accType,
-                        "prfId": self.__profileId,
-                        "delGrp" : GroupNames
-                        }
-        LOGGER.debug(f"_deleteGroups method is called with data : {request_body}")
-        response = self.__deleteGroupsAPI(url, json.dumps(request_body))
-        if response :
-            formatted_resp = WatchlistResource(response)._getWatchlistFormatted()._response
-            return formatted_resp
-        return response
-
-    def _renameGroup(self, GroupName : str, NewGroupName : str) -> str :
-        LOGGER.debug("inside _renameGroup method")
-
-        oldSymbols = None
-        oldGroupSymbolsResponse = self._getScripsOfGroup(GroupName)
-        if oldGroupSymbolsResponse :
-            oldSymRespDict = json.loads(oldGroupSymbolsResponse)
-            symList = oldSymRespDict.get('data').get('syLst')
-            if symList:
-                oldSymbols = [scrip.get('sym') for scrip in symList if scrip.get('sym')]
-
-        if not oldSymbols:
-            LOGGER.error("Failed to retrieve old group data. Please try again.")
-            print("Failed to retrieve old group data. Please try again.")
-            raise SystemExit(1)
-
-        currentUnixTimeStamp = int(time.time()*1000)
-
-        url = self.__routerObj._WatchlistGroupNameURL().format(groupName = GroupName)
-        request_body = {
-                        "accId": self.__accId,
-                        "accTyp": self.__accType,
-                        "act": "modify",
-                        "grpNm": GroupName,
-                        "newGrpNm": NewGroupName,
-                        "symLst": oldSymbols,
-                        "updatedOn" : currentUnixTimeStamp
-                        }
-
-        LOGGER.debug(f"_renameGroup method is called with data : {request_body}")
-        response = self.__renameGroupAPI(url, json.dumps(request_body))
-        if response :
-            return WatchlistResource(response)._getWatchlistFormatted()._response
-        return response
-
-    def __getUserAccData(self) :
-
-        # if user has eq acc id (acc type is EQ or COMEQ)
-        if self.__constants.eqAccId :
-            self.__accId = self.__constants.eqAccId
-            self.__accType = 'EQ'
-        # if user has co acc id (acc type is CO)
-        elif self.__constants.coAccId :
-            self.__accId = self.__constants.coAccId
-            self.__accType = 'CO'
-
-        self.__profileId = self.__constants.ProfileId
-
-    def __getGroupsWatchlistAPI(self, url : str, queryParams) -> str:
-
-        LOGGER.debug("inside __getGroupsWatchlistAPI method")
-
-        reply = self.__http._GetMethod(url, queryParams)
-
-        if reply :
-            reply = json.dumps(reply)
-        LOGGER.debug(f"Response received : {reply}")
-        return reply
-
-    def __getScripsOfGroupAPI(self, url : str, queryParams) -> str:
-
-        LOGGER.debug("inside __getScripsOfGroupAPI method")
-
-        reply = self.__http._GetMethod(url, queryParams)
-
-        if reply :
-            reply = json.dumps(reply)
-        LOGGER.debug(f"Response received : {reply}")
-        return reply
-
-    def __createGroupAPI(self, url : str, request_body : str) -> str:
-
-        LOGGER.debug("inside __createGroupAPI method")
-
-        reply = self.__http._PostMethod(url, request_body)
-
-        if reply :
-            reply = json.dumps(reply)
-        LOGGER.debug(f"Response received : {reply}")
-        return reply
-
-    def __addSymbolAPI(self, url : str, request_body : str) -> str:
-
-        LOGGER.debug("inside __addSymbolAPI method")
-
-        reply = self.__http._PutMethod(url, request_body)
-
-        if reply :
-            reply = json.dumps(reply)
-        LOGGER.debug(f"Response received : {reply}")
-        return reply
-
-    def __deleteSymbolAPI(self, url : str, request_body : str) -> str:
-
-        LOGGER.debug("inside __deleteSymbolAPI method")
-
-        reply = self.__http._PutMethod(url, request_body)
-
-        if reply :
-            reply = json.dumps(reply)
-        LOGGER.debug(f"Response received : {reply}")
-        return reply
-
-    def __deleteGroupsAPI(self, url : str, request_body : str) -> str:
-
-        LOGGER.debug("inside __deleteGroupsAPI method")
-
-        reply = self.__http._DeleteMethod(url, request_body)
-
-        if reply :
-            reply = json.dumps(reply)
-        LOGGER.debug(f"Response received : {reply}")
-        return reply
-
-    def __renameGroupAPI(self, url : str, request_body : str) -> str:
-
-        LOGGER.debug("inside __renameGroupAPI method")
-
-        reply = self.__http._PutMethod(url, request_body)
-
-        if reply :
-            reply = json.dumps(reply)
-        LOGGER.debug(f"Response received : {reply}")
-        return reply
+import json
+import logging
+import sys
+import time
+from typing import List
+from APIConnect.api_constants import ApiConstants
+from APIConnect.http import Http
+from constants.router import Router
+from resources.watchlist_resource import WatchlistResource
+
+LOGGER = logging.getLogger(__name__)
+
+class WatchlistService:
+    def __init__(self, routerObj, httpObj, constantsObj) -> None:
+        LOGGER.debug("WatchlistService object is being created.")
+
+        self.__routerObj : Router = routerObj
+        self.__http : Http = httpObj
+        self.__constants : ApiConstants = constantsObj
+        self.__accId = None
+        self.__accType = None
+        self.__profileId = None
+
+    def _getWatchlistGroups(self) -> str :
+        LOGGER.debug("inside _getWatchlistGroups method")
+
+        self.__getUserAccData()
+
+        url = self.__routerObj._WatchlistBaseGroupsURL()
+        queryParams = {"accId" : self.__accId, "accTyp" : self.__accType}
+
+        response = self.__getGroupsWatchlistAPI(url, queryParams)
+        if response :
+            formatted_resp = WatchlistResource(response)._getWatchlistFormatted()._response
+            return formatted_resp
+        return response
+
+    def _getScripsOfGroup(self, GroupName : str) -> str :
+        LOGGER.debug("inside _getScripsOfGroup method")
+
+        self.__getUserAccData()
+
+        url = self.__routerObj._WatchlistGetScripsURL()
+        queryParams = {"accId" : self.__accId, "accTyp" : self.__accType, "prfId" : self.__profileId, "grpNm" : GroupName}
+
+        response = self.__getScripsOfGroupAPI(url, queryParams)
+        if response :
+            formatted_resp = WatchlistResource(response)._getWatchlistFormatted()._response
+            return formatted_resp
+        return response
+
+    def _createGroup(self, GroupName : str, Symbols : List[str]) -> str :
+        LOGGER.debug("inside _createGroup method")
+
+        self.__getUserAccData()
+
+        url = self.__routerObj._WatchlistGroupNameURL().format(groupName = GroupName)
+        request_body = {
+                        "accId": self.__accId,
+                        "accTyp": self.__accType,
+                        "prfId": self.__profileId,
+                        "grpNm": GroupName,
+                        "symLst": Symbols
+                        }
+        LOGGER.debug(f"_createGroup method is called with data : {request_body}")
+        response = self.__createGroupAPI(url, json.dumps(request_body))
+        if response :
+            formatted_resp = WatchlistResource(response)._getWatchlistFormatted()._response
+            return formatted_resp
+        return response
+
+    def _addSymbols(self, GroupName : str, Symbols : List[str]) -> str :
+        LOGGER.debug("inside _addSymbol method")
+
+        self.__getUserAccData()
+        currentUnixTimeStamp = int(time.time()*1000)
+
+        url = self.__routerObj._WatchlistGroupNameURL().format(groupName = GroupName)
+        request_body = {
+                        "accId": self.__accId,
+                        "accTyp": self.__accType,
+                        "act": "add",
+                        "grpNm": GroupName,
+                        "symLst": Symbols,
+                        "updatedOn" : currentUnixTimeStamp
+                        }
+        LOGGER.debug(f"_addSymbol method is called with data : {request_body}")
+        response = self.__addSymbolAPI(url, json.dumps(request_body))
+        if response :
+            formatted_resp = WatchlistResource(response)._getWatchlistFormatted()._response
+            return formatted_resp
+        return response
+
+    def _deleteSymbols(self, GroupName : str, Symbols : List[str]) -> str :
+        LOGGER.debug("inside _deleteSymbols method")
+
+        self.__getUserAccData()
+        currentUnixTimeStamp = int(time.time()*1000)
+
+        url = self.__routerObj._WatchlistGroupNameURL().format(groupName = GroupName)
+        request_body = {
+                        "accId": self.__accId,
+                        "accTyp": self.__accType,
+                        "act": "del",
+                        "grpNm": GroupName,
+                        "symLst": Symbols,
+                        "updatedOn" : currentUnixTimeStamp
+                        }
+        LOGGER.debug(f"_deleteSymbols method is called with data : {request_body}")
+        response = self.__deleteSymbolAPI(url, json.dumps(request_body))
+        if response :
+            formatted_resp = WatchlistResource(response)._getWatchlistFormatted()._response
+            return formatted_resp
+        return response
+
+    def _deleteGroups(self, GroupNames : List[str]) -> str :
+        LOGGER.debug("inside _deleteGroups method")
+
+        self.__getUserAccData()
+
+        url = self.__routerObj._WatchlistBaseGroupsURL()
+        request_body = {
+                        "accId": self.__accId,
+                        "accTyp": self.__accType,
+                        "prfId": self.__profileId,
+                        "delGrp" : GroupNames
+                        }
+        LOGGER.debug(f"_deleteGroups method is called with data : {request_body}")
+        response = self.__deleteGroupsAPI(url, json.dumps(request_body))
+        if response :
+            formatted_resp = WatchlistResource(response)._getWatchlistFormatted()._response
+            return formatted_resp
+        return response
+
+    def _renameGroup(self, GroupName : str, NewGroupName : str) -> str :
+        LOGGER.debug("inside _renameGroup method")
+
+        oldSymbols = None
+        oldGroupSymbolsResponse = self._getScripsOfGroup(GroupName)
+        if oldGroupSymbolsResponse :
+            oldSymRespDict = json.loads(oldGroupSymbolsResponse)
+            symList = oldSymRespDict.get('data').get('syLst')
+            if symList:
+                oldSymbols = [scrip.get('sym') for scrip in symList if scrip.get('sym')]
+
+        if not oldSymbols:
+            LOGGER.error("Failed to retrieve old group data. Please try again.")
+            print("Failed to retrieve old group data. Please try again.")
+            raise SystemExit(1)
+
+        currentUnixTimeStamp = int(time.time()*1000)
+
+        url = self.__routerObj._WatchlistGroupNameURL().format(groupName = GroupName)
+        request_body = {
+                        "accId": self.__accId,
+                        "accTyp": self.__accType,
+                        "act": "modify",
+                        "grpNm": GroupName,
+                        "newGrpNm": NewGroupName,
+                        "symLst": oldSymbols,
+                        "updatedOn" : currentUnixTimeStamp
+                        }
+
+        LOGGER.debug(f"_renameGroup method is called with data : {request_body}")
+        response = self.__renameGroupAPI(url, json.dumps(request_body))
+        if response :
+            return WatchlistResource(response)._getWatchlistFormatted()._response
+        return response
+
+    def __getUserAccData(self) :
+
+        # if user has eq acc id (acc type is EQ or COMEQ)
+        if self.__constants.eqAccId :
+            self.__accId = self.__constants.eqAccId
+            self.__accType = 'EQ'
+        # if user has co acc id (acc type is CO)
+        elif self.__constants.coAccId :
+            self.__accId = self.__constants.coAccId
+            self.__accType = 'CO'
+
+        self.__profileId = self.__constants.ProfileId
+
+    def __getGroupsWatchlistAPI(self, url : str, queryParams) -> str:
+
+        LOGGER.debug("inside __getGroupsWatchlistAPI method")
+
+        reply = self.__http._GetMethod(url, queryParams)
+
+        if reply :
+            reply = json.dumps(reply)
+        LOGGER.debug(f"Response received : {reply}")
+        return reply
+
+    def __getScripsOfGroupAPI(self, url : str, queryParams) -> str:
+
+        LOGGER.debug("inside __getScripsOfGroupAPI method")
+
+        reply = self.__http._GetMethod(url, queryParams)
+
+        if reply :
+            reply = json.dumps(reply)
+        LOGGER.debug(f"Response received : {reply}")
+        return reply
+
+    def __createGroupAPI(self, url : str, request_body : str) -> str:
+
+        LOGGER.debug("inside __createGroupAPI method")
+
+        reply = self.__http._PostMethod(url, request_body)
+
+        if reply :
+            reply = json.dumps(reply)
+        LOGGER.debug(f"Response received : {reply}")
+        return reply
+
+    def __addSymbolAPI(self, url : str, request_body : str) -> str:
+
+        LOGGER.debug("inside __addSymbolAPI method")
+
+        reply = self.__http._PutMethod(url, request_body)
+
+        if reply :
+            reply = json.dumps(reply)
+        LOGGER.debug(f"Response received : {reply}")
+        return reply
+
+    def __deleteSymbolAPI(self, url : str, request_body : str) -> str:
+
+        LOGGER.debug("inside __deleteSymbolAPI method")
+
+        reply = self.__http._PutMethod(url, request_body)
+
+        if reply :
+            reply = json.dumps(reply)
+        LOGGER.debug(f"Response received : {reply}")
+        return reply
+
+    def __deleteGroupsAPI(self, url : str, request_body : str) -> str:
+
+        LOGGER.debug("inside __deleteGroupsAPI method")
+
+        reply = self.__http._DeleteMethod(url, request_body)
+
+        if reply :
+            reply = json.dumps(reply)
+        LOGGER.debug(f"Response received : {reply}")
+        return reply
+
+    def __renameGroupAPI(self, url : str, request_body : str) -> str:
+
+        LOGGER.debug("inside __renameGroupAPI method")
+
+        reply = self.__http._PutMethod(url, request_body)
+
+        if reply :
+            reply = json.dumps(reply)
+        LOGGER.debug(f"Response received : {reply}")
+        return reply
```

### Comparing `APIConnect-2.0.1.post1/setup.py` & `APIConnect-2.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from setuptools import setup
-setup(
-    name='APIConnect',
-    packages=['APIConnect', 'constants', 'exceptions', 'resources', 'services', 'feed'],
-    version='2.0.1.post1',
-    license='MIT',
-    description='APIs to trade from Nuvama',
-    author='Nuvama',
-    author_email='support@nuvama.com',
-    url='https://nuvamawealth.com/',
-    download_url='https://www.nuvamawealth.com/ewwebimages/webfiles/download/Python_APIConnect/APIConnect-2.0.1.post1.tar.gz',
-    keywords=['Nuvama', 'Open API', 'Trade', 'Nuvama Python Library'],
-    python_requires=">=3.7",
-    install_requires=[
-        'urllib3>=1.26.6',
-        'requests>=2.26.0'
-        ],
-    data_files=[('conf',['conf/settings.ini'])],
-    license_files = ['LICENSE.txt',],
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
-    ],
+from setuptools import setup
+
+setup(
+    name='APIConnect',
+    packages=['APIConnect', 'constants', 'exceptions', 'resources', 'services', 'feed'],
+    version='2.0.2',
+    license='MIT',
+    description='APIs to trade from Nuvama',
+    author='Nuvama',
+    author_email='support@nuvama.com',
+    url='https://nuvamawealth.com/',
+    download_url='https://www.nuvamawealth.com/ewwebimages/webfiles/download/Python_APIConnect/APIConnect-2.0.2.tar.gz',
+    keywords=['Nuvama', 'Open API', 'Trade', 'Nuvama Python Library'],
+    python_requires=">=3.7",
+    install_requires=[
+        'urllib3>=1.26.6',
+        'requests>=2.26.0'
+        ],
+    data_files=[('conf',['conf/settings.ini'])],
+    license_files = ['LICENSE.txt',],
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3 :: Only',
+        'Programming Language :: Python :: 3.7',
+    ],
 )
```

