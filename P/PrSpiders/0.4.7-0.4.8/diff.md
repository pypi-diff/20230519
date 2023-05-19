# Comparing `tmp/PrSpiders-0.4.7.tar.gz` & `tmp/PrSpiders-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.4.7.tar", last modified: Thu May 18 01:00:05 2023, max compression
+gzip compressed data, was "PrSpiders-0.4.8.tar", last modified: Fri May 19 08:09:35 2023, max compression
```

## Comparing `PrSpiders-0.4.7.tar` & `PrSpiders-0.4.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 01:00:05.642360 PrSpiders-0.4.7/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.4.7/LICENSE.txt
--rw-rw-rw-   0        0        0     5678 2023-05-18 01:00:05.639362 PrSpiders-0.4.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 01:00:05.407361 PrSpiders-0.4.7/PrSpider/
--rw-rw-rw-   0        0        0    12766 2023-05-18 00:59:32.000000 PrSpiders-0.4.7/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       79 2023-05-17 09:01:20.000000 PrSpiders-0.4.7/PrSpider/__init__.py
--rw-rw-rw-   0        0        0    11041 2023-05-17 12:26:30.000000 PrSpiders-0.4.7/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     4527 2023-05-17 12:26:04.000000 PrSpiders-0.4.7/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.7/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-05-18 01:00:05.490362 PrSpiders-0.4.7/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     5678 2023-05-18 01:00:04.000000 PrSpiders-0.4.7/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      563 2023-05-18 01:00:05.000000 PrSpiders-0.4.7/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 01:00:04.000000 PrSpiders-0.4.7/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-18 01:00:04.000000 PrSpiders-0.4.7/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-05-18 01:00:04.000000 PrSpiders-0.4.7/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-18 01:00:04.000000 PrSpiders-0.4.7/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5166 2023-04-23 08:22:29.000000 PrSpiders-0.4.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 01:00:05.505365 PrSpiders-0.4.7/pkg/
--rw-rw-rw-   0        0        0       23 2023-04-23 03:23:07.000000 PrSpiders-0.4.7/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 01:00:05.568361 PrSpiders-0.4.7/pkg/prspider/
--rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.4.7/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.4.7/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.4.7/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.4.7/pkg/prspider/start.py
-drwxrwxrwx   0        0        0        0 2023-05-18 01:00:05.623365 PrSpiders-0.4.7/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.4.7/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.4.7/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.4.7/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.7/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-05-18 01:00:05.643360 PrSpiders-0.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1022 2023-05-18 01:00:00.000000 PrSpiders-0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:09:35.111789 PrSpiders-0.4.8/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.4.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     5678 2023-05-19 08:09:35.107789 PrSpiders-0.4.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-19 08:09:34.836786 PrSpiders-0.4.8/PrSpider/
+-rw-rw-rw-   0        0        0    12713 2023-05-18 01:02:32.000000 PrSpiders-0.4.8/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       79 2023-05-17 09:01:20.000000 PrSpiders-0.4.8/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0    11011 2023-05-19 08:04:11.000000 PrSpiders-0.4.8/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     4468 2023-05-18 02:26:44.000000 PrSpiders-0.4.8/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.8/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:09:34.917788 PrSpiders-0.4.8/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     5678 2023-05-19 08:09:34.000000 PrSpiders-0.4.8/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      563 2023-05-19 08:09:34.000000 PrSpiders-0.4.8/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 08:09:34.000000 PrSpiders-0.4.8/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-19 08:09:34.000000 PrSpiders-0.4.8/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-05-19 08:09:34.000000 PrSpiders-0.4.8/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-19 08:09:34.000000 PrSpiders-0.4.8/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5166 2023-04-23 08:22:29.000000 PrSpiders-0.4.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 08:09:34.935788 PrSpiders-0.4.8/pkg/
+-rw-rw-rw-   0        0        0       23 2023-04-23 03:23:07.000000 PrSpiders-0.4.8/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:09:35.013786 PrSpiders-0.4.8/pkg/prspider/
+-rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.4.8/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.4.8/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.4.8/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.4.8/pkg/prspider/start.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:09:35.080802 PrSpiders-0.4.8/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.4.8/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.4.8/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.4.8/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.8/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-05-19 08:09:35.112786 PrSpiders-0.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2023-05-19 08:09:27.000000 PrSpiders-0.4.8/setup.py
```

### Comparing `PrSpiders-0.4.7/LICENSE.txt` & `PrSpiders-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.7/PKG-INFO` & `PrSpiders-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.4.7
+Version: 0.4.8
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.4.7/PrSpider/PrSpiders.py` & `PrSpiders-0.4.8/PrSpider/PrSpiders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import os
 import re
 import sys
 import time
-import datetime, random
 from typing import Optional
 from loguru import logger as loguer
 from .requestXpath import prequest
 from concurrent.futures import ThreadPoolExecutor, as_completed
-from rich.text import Text
 
 
 class settions(object):
     workers: Optional[int] = 10000
     request_num: Optional[int] = 0
     retry_num: Optional[int] = 0
     success_num: Optional[int] = 0
```

### Comparing `PrSpiders-0.4.7/PrSpider/pxpath.py` & `PrSpiders-0.4.8/PrSpider/pxpath.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from urllib.parse import urljoin
 import re, time, copy
 from lxml import etree
 from datetime import timedelta, datetime
 import unicodedata
-from .PrSpiders import loguer
 
 
 class Xpath(object):
     def __init__(self, response, encoding="utf-8"):
         if isinstance(response, str):
             self.res = etree.HTML(response)
         else:
@@ -129,15 +128,15 @@
         """
         :param lists: 是否返回列表,True返回列表
         :param warps: 换行符合 0*\n
         :param repl: 文本进行格式化
         :return:  返回解析文本的字符串或者列表
         """
         text_xpath = ".//text()"
-        if "text()" in self._expr:
+        if "/text()" in self._expr:
             return self.xp
         warps = "\n" * warps
         if isinstance(self.xp, list):
             self.result = [_.xpath(text_xpath) for _ in self.xp]
             if lists is False:
                 self.result = (
                     [f"{warps}".join([replace(i) for i in _]) for _ in self.result]
```

### Comparing `PrSpiders-0.4.7/PrSpider/requestXpath.py` & `PrSpiders-0.4.8/PrSpider/requestXpath.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from requests.exceptions import SSLError
 import requests
 import time
 import json
 from requests.models import Response
 from .useragent import get_ua
 from .pxpath import Xpath
-import datetime
 
 """
 -------------------------------------------------
    File Name:     prequest
    Description :   Network Requests Class
    Author :        penr
    date:          2023/02/16
```

### Comparing `PrSpiders-0.4.7/PrSpider/useragent.py` & `PrSpiders-0.4.8/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.7/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.4.8/PrSpiders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.4.7
+Version: 0.4.8
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.4.7/PrSpiders.egg-info/SOURCES.txt` & `PrSpiders-0.4.8/PrSpiders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.7/README.md` & `PrSpiders-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.7/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.4.8/pkg/prspider/PrSpider_CMD.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.7/pkg/prspider/start.py` & `PrSpiders-0.4.8/pkg/prspider/start.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.7/requestXpath/__init__.py` & `PrSpiders-0.4.8/requestXpath/__init__.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.7/requestXpath/pxpath.py` & `PrSpiders-0.4.8/requestXpath/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.7/requestXpath/requestXpath.py` & `PrSpiders-0.4.8/requestXpath/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.7/requestXpath/useragent.py` & `PrSpiders-0.4.8/requestXpath/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.7/setup.py` & `PrSpiders-0.4.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
 
-__version__ = "0.4.7"
+__version__ = "0.4.8"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
@@ -15,15 +15,15 @@
     author_email="1944542244@qq.com",
     description="Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/peng0928/prequests",
     packages=find_packages(),
-    install_requires=["requests", "urllib3", "lxml", "xpinyin", "PrSpiders"],
+    install_requires=["requests", "urllib3", "lxml", "xpinyin", "PrSpiders", 'loguru'],
     entry_points={"console_scripts": ["prspiders = pkg.prspider.PrSpider_CMD:main"]},
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
 )
```

