# Comparing `tmp/pyCryptomusAPI-0.0.3.tar.gz` & `tmp/pyCryptomusAPI-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyCryptomusAPI-0.0.3.tar", last modified: Sun Apr  9 09:10:02 2023, max compression
+gzip compressed data, was "pyCryptomusAPI-0.0.4.tar", last modified: Fri May 19 20:20:37 2023, max compression
```

## Comparing `pyCryptomusAPI-0.0.3.tar` & `pyCryptomusAPI-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 09:10:02.958784 pyCryptomusAPI-0.0.3/
--rw-rw-rw-   0        0        0     1085 2022-12-10 18:10:42.000000 pyCryptomusAPI-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2174 2023-04-09 09:10:02.958784 pyCryptomusAPI-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1672 2022-12-12 17:35:04.000000 pyCryptomusAPI-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 09:10:02.958784 pyCryptomusAPI-0.0.3/pyCryptomusAPI/
--rw-rw-rw-   0        0        0       20 2022-12-10 22:13:53.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI/__init__.py
--rw-rw-rw-   0        0        0    17058 2023-04-09 09:06:52.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI/api.py
--rw-rw-rw-   0        0        0     9897 2023-01-21 14:08:46.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI/cryto_types.py
--rw-rw-rw-   0        0        0      374 2023-02-14 14:49:00.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI/private_keys.py
--rw-rw-rw-   0        0        0     2314 2023-02-14 14:48:55.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI/tests.py
--rw-rw-rw-   0        0        0       95 2023-04-09 09:05:01.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI/version.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:10:02.958784 pyCryptomusAPI-0.0.3/pyCryptomusAPI.egg-info/
--rw-rw-rw-   0        0        0     2174 2023-04-09 09:10:02.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-04-09 09:10:02.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 09:10:02.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-09 09:10:02.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 09:10:02.958784 pyCryptomusAPI-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1053 2022-12-10 18:13:01.000000 pyCryptomusAPI-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 20:20:37.759322 pyCryptomusAPI-0.0.4/
+-rw-rw-rw-   0        0        0     1085 2022-12-10 18:10:42.000000 pyCryptomusAPI-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2174 2023-05-19 20:20:37.757723 pyCryptomusAPI-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1672 2022-12-12 17:35:04.000000 pyCryptomusAPI-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 20:20:37.749248 pyCryptomusAPI-0.0.4/pyCryptomusAPI/
+-rw-rw-rw-   0        0        0       20 2022-12-10 22:13:53.000000 pyCryptomusAPI-0.0.4/pyCryptomusAPI/__init__.py
+-rw-rw-rw-   0        0        0    17334 2023-05-19 20:09:41.000000 pyCryptomusAPI-0.0.4/pyCryptomusAPI/api.py
+-rw-rw-rw-   0        0        0     9897 2023-01-21 14:08:46.000000 pyCryptomusAPI-0.0.4/pyCryptomusAPI/cryto_types.py
+-rw-rw-rw-   0        0        0      374 2023-02-14 14:49:00.000000 pyCryptomusAPI-0.0.4/pyCryptomusAPI/private_keys.py
+-rw-rw-rw-   0        0        0     2314 2023-02-14 14:48:55.000000 pyCryptomusAPI-0.0.4/pyCryptomusAPI/tests.py
+-rw-rw-rw-   0        0        0       95 2023-05-19 20:11:15.000000 pyCryptomusAPI-0.0.4/pyCryptomusAPI/version.py
+drwxrwxrwx   0        0        0        0 2023-05-19 20:20:37.756723 pyCryptomusAPI-0.0.4/pyCryptomusAPI.egg-info/
+-rw-rw-rw-   0        0        0     2174 2023-05-19 20:20:37.000000 pyCryptomusAPI-0.0.4/pyCryptomusAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-05-19 20:20:37.000000 pyCryptomusAPI-0.0.4/pyCryptomusAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 20:20:37.000000 pyCryptomusAPI-0.0.4/pyCryptomusAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-19 20:20:37.000000 pyCryptomusAPI-0.0.4/pyCryptomusAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 20:20:37.759322 pyCryptomusAPI-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2022-12-10 18:13:01.000000 pyCryptomusAPI-0.0.4/setup.py
```

### Comparing `pyCryptomusAPI-0.0.3/LICENSE` & `pyCryptomusAPI-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyCryptomusAPI-0.0.3/PKG-INFO` & `pyCryptomusAPI-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCryptomusAPI
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python implementation of Cryptomus (https://cryptomus.com) pubilc API
 Home-page: https://github.com/Badiboy/pyCryptomusAPI
 Author: Badiboy
 License: MIT license
 Keywords: Crypto Pay API Cryptomus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyCryptomusAPI-0.0.3/README.md` & `pyCryptomusAPI-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyCryptomusAPI-0.0.3/pyCryptomusAPI/api.py` & `pyCryptomusAPI-0.0.4/pyCryptomusAPI/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,31 @@
 class pyCryptomusAPI:
     """
     Cryptomus API Client
     """
 
     def __init__(self,
                  merchant_uuid, payment_api_key = None, payout_api_key = None,
-                 print_errors = False, timeout = None):
+                 print_errors = False, timeout = None, add_request_params = None):
         """
         Create the pyCryptomusAPI instance.
 
         :param merchant_uuid: The merchant's uuid, which you can find in the merchant's personal account in the settings section.
         :param payment_api_key: API key for processing payments
         :param payout_api_key: API key for accepting payment and making payouts
         :param print_errors: (Optional) Print dumps on request errors
         :param timeout: (Optional) Request timeout
+        :param add_request_params: (List, Optional) Additional request parameters to pass with API calls
         """
         self.merchant_uuid = merchant_uuid
         self.payment_api_key = payment_api_key
         self.payout_api_key = payout_api_key
         self.print_errors = print_errors
         self.timeout = timeout
+        self.add_request_params = add_request_params
         if not(self.payment_api_key) and not(self.payout_api_key):
             raise Exception("You must specify at least one API key.")
 
     def __request(self, method_url, mode, **kwargs):
         """
         Send request to API
 
@@ -52,14 +54,17 @@
         :param kwargs: request data
         """
         if kwargs:
             data = dict(kwargs)
         else:
             data = {}
 
+        if self.add_request_params:
+            data.update(self.add_request_params)
+
         base_resp = None
         try:
             key = self.payment_api_key if (mode == 1) else self.payout_api_key
             json_dumps = json.dumps(data)
             # json_dumps = json.dumps(data, ensure_ascii=False, separators=(',', ':'))
             pre_sign = json_dumps if data else ""
             sign = md5(base64.b64encode(pre_sign.encode('ascii')) + key.encode('ascii')).hexdigest()
```

### Comparing `pyCryptomusAPI-0.0.3/pyCryptomusAPI/cryto_types.py` & `pyCryptomusAPI-0.0.4/pyCryptomusAPI/cryto_types.py`

 * *Files identical despite different names*

### Comparing `pyCryptomusAPI-0.0.3/pyCryptomusAPI/tests.py` & `pyCryptomusAPI-0.0.4/pyCryptomusAPI/tests.py`

 * *Files identical despite different names*

### Comparing `pyCryptomusAPI-0.0.3/pyCryptomusAPI.egg-info/PKG-INFO` & `pyCryptomusAPI-0.0.4/pyCryptomusAPI.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCryptomusAPI
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python implementation of Cryptomus (https://cryptomus.com) pubilc API
 Home-page: https://github.com/Badiboy/pyCryptomusAPI
 Author: Badiboy
 License: MIT license
 Keywords: Crypto Pay API Cryptomus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyCryptomusAPI-0.0.3/setup.py` & `pyCryptomusAPI-0.0.4/setup.py`

 * *Files identical despite different names*

