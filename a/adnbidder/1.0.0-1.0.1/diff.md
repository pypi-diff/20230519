# Comparing `tmp/adnbidder-1.0.0.tar.gz` & `tmp/adnbidder-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adnbidder-1.0.0.tar", last modified: Fri May 19 00:51:24 2023, max compression
+gzip compressed data, was "adnbidder-1.0.1.tar", last modified: Fri May 19 01:34:20 2023, max compression
```

## Comparing `adnbidder-1.0.0.tar` & `adnbidder-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 richardmasterton   (501) staff       (20)        0 2023-05-19 00:51:24.468700 adnbidder-1.0.0/
--rw-r--r--   0 richardmasterton   (501) staff       (20)     1068 2022-07-25 23:31:29.000000 adnbidder-1.0.0/LICENSE.txt
--rw-r--r--   0 richardmasterton   (501) staff       (20)      484 2023-05-19 00:51:24.468472 adnbidder-1.0.0/PKG-INFO
--rw-r--r--   0 richardmasterton   (501) staff       (20)      996 2023-05-18 23:28:24.000000 adnbidder-1.0.0/README.md
-drwxr-xr-x   0 richardmasterton   (501) staff       (20)        0 2023-05-19 00:51:24.467433 adnbidder-1.0.0/adnbidder/
--rw-r--r--   0 richardmasterton   (501) staff       (20)       22 2023-05-17 20:31:23.000000 adnbidder-1.0.0/adnbidder/__init__.py
--rw-r--r--   0 richardmasterton   (501) staff       (20)    13042 2023-05-19 00:43:54.000000 adnbidder-1.0.0/adnbidder/bidder.py
-drwxr-xr-x   0 richardmasterton   (501) staff       (20)        0 2023-05-19 00:51:24.468295 adnbidder-1.0.0/adnbidder.egg-info/
--rw-r--r--   0 richardmasterton   (501) staff       (20)      484 2023-05-19 00:51:24.000000 adnbidder-1.0.0/adnbidder.egg-info/PKG-INFO
--rw-r--r--   0 richardmasterton   (501) staff       (20)      236 2023-05-19 00:51:24.000000 adnbidder-1.0.0/adnbidder.egg-info/SOURCES.txt
--rw-r--r--   0 richardmasterton   (501) staff       (20)        1 2023-05-19 00:51:24.000000 adnbidder-1.0.0/adnbidder.egg-info/dependency_links.txt
--rw-r--r--   0 richardmasterton   (501) staff       (20)       26 2023-05-19 00:51:24.000000 adnbidder-1.0.0/adnbidder.egg-info/requires.txt
--rw-r--r--   0 richardmasterton   (501) staff       (20)       10 2023-05-19 00:51:24.000000 adnbidder-1.0.0/adnbidder.egg-info/top_level.txt
--rw-r--r--   0 richardmasterton   (501) staff       (20)       38 2023-05-19 00:51:24.468736 adnbidder-1.0.0/setup.cfg
--rw-r--r--   0 richardmasterton   (501) staff       (20)      737 2023-05-19 00:41:23.000000 adnbidder-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:34:20.150368 adnbidder-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 01:34:09.000000 adnbidder-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-19 01:34:20.150368 adnbidder-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-19 01:34:09.000000 adnbidder-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:34:20.150368 adnbidder-1.0.1/adnbidder/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 01:34:09.000000 adnbidder-1.0.1/adnbidder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-05-19 01:34:09.000000 adnbidder-1.0.1/adnbidder/bidder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:34:20.150368 adnbidder-1.0.1/adnbidder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-19 01:34:20.000000 adnbidder-1.0.1/adnbidder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-19 01:34:20.000000 adnbidder-1.0.1/adnbidder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 01:34:20.000000 adnbidder-1.0.1/adnbidder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-19 01:34:20.000000 adnbidder-1.0.1/adnbidder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 01:34:20.000000 adnbidder-1.0.1/adnbidder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 01:34:20.150368 adnbidder-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-19 01:34:09.000000 adnbidder-1.0.1/setup.py
```

### Comparing `adnbidder-1.0.0/LICENSE.txt` & `adnbidder-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adnbidder-1.0.0/README.md` & `adnbidder-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `adnbidder-1.0.0/adnbidder/bidder.py` & `adnbidder-1.0.1/adnbidder/bidder.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,17 +122,15 @@
             line_item_id = line_item
             line_item = self.api_client.line_items.get(line_item_id)
         line_item_stats = LineItemBidStats(self.api_client, line_item)
         for bid_update in self.get_line_item_bid_updates(line_item, line_item_stats):
             try:
                 self.api_client.bidding.update(bid_update.to_payload())
             except RuntimeError as err:
-                # The Adnuntius API module reports API errors a RuntimeErrors.
-                # Just log the error and keep the bidder going
-                print(err)
+                self.bid_error_handler(err)
 
     def get_line_item_bid_updates(self, line_item, line_item_stats):
         """
         This is the heart of the bidding control algorithm. Custom bidder implementations
         should override this method to provide custom bidding decisions in their adaptor.
         :param line_item: The Line Item object
         :param line_item_stats: The bid data for the Line Item across all the Sites where it runs.
@@ -169,15 +167,15 @@
                         bid_update = BidUpdate(line_item_stats.line_item_id,
                                                site_bid.site_id,
                                                bid.bid_cpm)
                         bid_updates.append(bid_update)
                         break
         return bid_updates
 
-    def shutdown(self, sig, frame):
+    def shutdown(self, sig=None, frame=None):
         """
         Shuts down the bidder immediately
         :param sig:
         :param frame:
         :return:
         """
         print('Shutting down bidder...')
@@ -187,14 +185,23 @@
         """
         A method stub that can be overridden by child classes.
         This method will be called once per cycle in the main service loop.
         :return:
         """
         return self
 
+    def bid_error_handler(self, error):
+        """
+        This method will be called if there is an error sending a bid update.
+        Should be overriden by custom bidders if you don't want to shut down on any error.
+        :return:
+        """
+        print(error)
+        self.shutdown()
+
 
 class BidWinRate:
     """
     Structure for holding a bid CPM and observed win rate.
     """
     def __init__(self, bid_win_rate):
         self.bid_cpm = bid_win_rate['bidCpm']
```

### Comparing `adnbidder-1.0.0/setup.py` & `adnbidder-1.0.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pathlib
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 setup(
     name="adnbidder",
-    version="1.0.0",
+    version="1.0.1",
     description="A simple client for controlling bidding in the Adnuntius platform",
     long_description="A simple client for controlling bidding in the Adnuntius platform",
-    url="https://github.com/Adnuntius/adnbidder",
+    url="https://github.com/Adnuntius/adnuntius-bidder",
     author="Adnuntius",
     author_email="tech@adnuntius.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
```

