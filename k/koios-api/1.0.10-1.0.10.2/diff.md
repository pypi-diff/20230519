# Comparing `tmp/koios-api-1.0.10.tar.gz` & `tmp/koios-api-1.0.10.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koios-api-1.0.10.tar", last modified: Thu May 11 14:46:14 2023, max compression
+gzip compressed data, was "koios-api-1.0.10.2.tar", last modified: Fri May 19 08:41:21 2023, max compression
```

## Comparing `koios-api-1.0.10.tar` & `koios-api-1.0.10.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 14:46:14.787757 koios-api-1.0.10/
--rw-rw-r--   0 george    (1000) george    (1000)     1080 2023-04-22 10:04:11.000000 koios-api-1.0.10/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)   106198 2023-05-11 14:46:14.787757 koios-api-1.0.10/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)   105559 2023-05-11 14:23:40.000000 koios-api-1.0.10/README.md
--rw-rw-r--   0 george    (1000) george    (1000)      795 2023-05-11 12:09:00.000000 koios-api-1.0.10/pyproject.toml
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-11 14:46:14.787757 koios-api-1.0.10/setup.cfg
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 14:46:14.783757 koios-api-1.0.10/src/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 14:46:14.783757 koios-api-1.0.10/src/koios_api/
--rw-rw-r--   0 george    (1000) george    (1000)     1393 2023-05-11 12:12:45.000000 koios-api-1.0.10/src/koios_api/__config__.py
--rw-rw-r--   0 george    (1000) george    (1000)      228 2022-10-13 07:47:20.000000 koios-api-1.0.10/src/koios_api/__init__.py
--rw-rw-r--   0 george    (1000) george    (1000)    10489 2023-05-11 12:03:05.000000 koios-api-1.0.10/src/koios_api/account.py
--rw-rw-r--   0 george    (1000) george    (1000)     5649 2023-05-11 12:03:19.000000 koios-api-1.0.10/src/koios_api/address.py
--rw-rw-r--   0 george    (1000) george    (1000)    16024 2023-05-11 13:26:52.000000 koios-api-1.0.10/src/koios_api/asset.py
--rw-rw-r--   0 george    (1000) george    (1000)     3177 2023-05-11 12:03:49.000000 koios-api-1.0.10/src/koios_api/block.py
--rw-rw-r--   0 george    (1000) george    (1000)     2690 2023-05-11 08:51:55.000000 koios-api-1.0.10/src/koios_api/epoch.py
--rw-rw-r--   0 george    (1000) george    (1000)     2514 2023-05-11 08:41:06.000000 koios-api-1.0.10/src/koios_api/network.py
--rw-rw-r--   0 george    (1000) george    (1000)    10429 2023-05-11 12:04:12.000000 koios-api-1.0.10/src/koios_api/pool.py
--rw-rw-r--   0 george    (1000) george    (1000)     3595 2023-05-11 12:04:31.000000 koios-api-1.0.10/src/koios_api/script.py
--rw-rw-r--   0 george    (1000) george    (1000)     5414 2023-05-11 12:04:23.000000 koios-api-1.0.10/src/koios_api/transactions.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 14:46:14.783757 koios-api-1.0.10/src/koios_api.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)   106198 2023-05-11 14:46:14.000000 koios-api-1.0.10/src/koios_api.egg-info/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)      490 2023-05-11 14:46:14.000000 koios-api-1.0.10/src/koios_api.egg-info/SOURCES.txt
--rw-rw-r--   0 george    (1000) george    (1000)        1 2023-05-11 14:46:14.000000 koios-api-1.0.10/src/koios_api.egg-info/dependency_links.txt
--rw-rw-r--   0 george    (1000) george    (1000)       17 2023-05-11 14:46:14.000000 koios-api-1.0.10/src/koios_api.egg-info/requires.txt
--rw-rw-r--   0 george    (1000) george    (1000)       16 2023-05-11 14:46:14.000000 koios-api-1.0.10/src/koios_api.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-19 08:41:21.159385 koios-api-1.0.10.2/
+-rw-rw-r--   0 george    (1000) george    (1000)     1080 2023-04-22 10:04:11.000000 koios-api-1.0.10.2/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)   106197 2023-05-19 08:41:21.159385 koios-api-1.0.10.2/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)   105556 2023-05-19 07:45:13.000000 koios-api-1.0.10.2/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)      797 2023-05-19 08:38:22.000000 koios-api-1.0.10.2/pyproject.toml
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-19 08:41:21.159385 koios-api-1.0.10.2/setup.cfg
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-19 08:41:21.155384 koios-api-1.0.10.2/src/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-19 08:41:21.159385 koios-api-1.0.10.2/src/koios_api/
+-rw-rw-r--   0 george    (1000) george    (1000)     1393 2023-05-11 12:12:45.000000 koios-api-1.0.10.2/src/koios_api/__config__.py
+-rw-rw-r--   0 george    (1000) george    (1000)      228 2022-10-13 07:47:20.000000 koios-api-1.0.10.2/src/koios_api/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)    10489 2023-05-11 12:03:05.000000 koios-api-1.0.10.2/src/koios_api/account.py
+-rw-rw-r--   0 george    (1000) george    (1000)     5995 2023-05-18 15:33:57.000000 koios-api-1.0.10.2/src/koios_api/address.py
+-rw-rw-r--   0 george    (1000) george    (1000)    16024 2023-05-11 13:26:52.000000 koios-api-1.0.10.2/src/koios_api/asset.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3177 2023-05-11 12:03:49.000000 koios-api-1.0.10.2/src/koios_api/block.py
+-rw-rw-r--   0 george    (1000) george    (1000)     2690 2023-05-11 08:51:55.000000 koios-api-1.0.10.2/src/koios_api/epoch.py
+-rw-rw-r--   0 george    (1000) george    (1000)     2514 2023-05-11 08:41:06.000000 koios-api-1.0.10.2/src/koios_api/network.py
+-rw-rw-r--   0 george    (1000) george    (1000)    10428 2023-05-19 07:44:11.000000 koios-api-1.0.10.2/src/koios_api/pool.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3595 2023-05-11 12:04:31.000000 koios-api-1.0.10.2/src/koios_api/script.py
+-rw-rw-r--   0 george    (1000) george    (1000)     5414 2023-05-11 12:04:23.000000 koios-api-1.0.10.2/src/koios_api/transactions.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-19 08:41:21.159385 koios-api-1.0.10.2/src/koios_api.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)   106197 2023-05-19 08:41:21.000000 koios-api-1.0.10.2/src/koios_api.egg-info/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)      490 2023-05-19 08:41:21.000000 koios-api-1.0.10.2/src/koios_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 george    (1000) george    (1000)        1 2023-05-19 08:41:21.000000 koios-api-1.0.10.2/src/koios_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       17 2023-05-19 08:41:21.000000 koios-api-1.0.10.2/src/koios_api.egg-info/requires.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       16 2023-05-19 08:41:21.000000 koios-api-1.0.10.2/src/koios_api.egg-info/top_level.txt
```

### Comparing `koios-api-1.0.10/LICENSE` & `koios-api-1.0.10.2/LICENSE`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10/PKG-INFO` & `koios-api-1.0.10.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koios-api
-Version: 1.0.10
+Version: 1.0.10.2
 Summary: A python package for the Cardano Blockchain Koios API (https://api.koios.rest/)
 Author-email: APEX Stake Pool <cardanoapexpool@gmail.com>
 Project-URL: Homepage, https://github.com/cardano-apexpool/koios-api-python
 Project-URL: Bug Tracker, https://github.com/cardano-apexpool/koios-api-python/issues
 Keywords: koios,cardano,blockchain,REST,API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -111,15 +111,15 @@
 [get_policy_asset_addresses](#get_policy_asset_addresses) Get the list of addresses with quantity for each asset on the given policy<br>
 [get_policy_asset_info](#get_policy_asset_info) Get the information for all assets under the same policy<br>
 [get_policy_asset_list](#get_policy_asset_list) Get the list of asset under the given policy (including balances)<br>
 [get_asset_summary](#get_asset_summary) Get the summary of an asset (total transactions exclude minting/total wallets include only wallets with asset balance)<br>
 [get_asset_txs](#get_asset_txs) Get the list of all asset transaction hashes (the newest first)<br>
 
 [Pool](#Pool)<br>
-[get_pools_list](#get_pools_list) A list of all currently registered/retiring (not retired) pools<br>
+[get_pool_list](#get_pool_list) A list of all currently registered/retiring (not retired) pools<br>
 [get_pool_info](#get_pool_info) Current pool statuses and details for a specified list of pool ids<br>
 [get_pool_stake_snapshot](#get_pool_stake_snapshot) Returns Mark, Set and Go stake snapshots for the selected pool, useful for leaderlog calculation<br>
 [get_pool_delegators](#get_pool_delegators) Returns information about live delegators for a given pool<br>
 [get_pool_delegators_history](#get_pool_delegators_history) Returns information about active delegators (incl. history) for a given pool and epoch number (all epochs if not specified)<br>
 [get_pool_blocks](#get_pool_blocks) Returns information about blocks minted by a given pool for all epochs (or _epoch_no if provided)<br>
 [get_pool_history](#get_pool_history) Returns information about pool stake, block and reward history in a given epoch (or all epochs that pool existed for, in descending order if no epoch number was provided)<br>
 [get_pool_updates](#get_pool_updates) Returns all pool updates for all pools or only updates for specific pool if specified<br>
@@ -1558,15 +1558,15 @@
     "block_time": 1670493734
   }
 ]
 ```
 
 ### Pool
 
-#### get_pools_list
+#### get_pool_list
 A list of all currently registered/retiring (not retired) pools<br>
 Parameters: none<br>
 Returns: The list of stake pool dictionaries<br>
 Example:<br>
 `pool_list = get_pool_list()`<br>
 Example response:
 ```json
```

### Comparing `koios-api-1.0.10/README.md` & `koios-api-1.0.10.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 [get_policy_asset_addresses](#get_policy_asset_addresses) Get the list of addresses with quantity for each asset on the given policy<br>
 [get_policy_asset_info](#get_policy_asset_info) Get the information for all assets under the same policy<br>
 [get_policy_asset_list](#get_policy_asset_list) Get the list of asset under the given policy (including balances)<br>
 [get_asset_summary](#get_asset_summary) Get the summary of an asset (total transactions exclude minting/total wallets include only wallets with asset balance)<br>
 [get_asset_txs](#get_asset_txs) Get the list of all asset transaction hashes (the newest first)<br>
 
 [Pool](#Pool)<br>
-[get_pools_list](#get_pools_list) A list of all currently registered/retiring (not retired) pools<br>
+[get_pool_list](#get_pool_list) A list of all currently registered/retiring (not retired) pools<br>
 [get_pool_info](#get_pool_info) Current pool statuses and details for a specified list of pool ids<br>
 [get_pool_stake_snapshot](#get_pool_stake_snapshot) Returns Mark, Set and Go stake snapshots for the selected pool, useful for leaderlog calculation<br>
 [get_pool_delegators](#get_pool_delegators) Returns information about live delegators for a given pool<br>
 [get_pool_delegators_history](#get_pool_delegators_history) Returns information about active delegators (incl. history) for a given pool and epoch number (all epochs if not specified)<br>
 [get_pool_blocks](#get_pool_blocks) Returns information about blocks minted by a given pool for all epochs (or _epoch_no if provided)<br>
 [get_pool_history](#get_pool_history) Returns information about pool stake, block and reward history in a given epoch (or all epochs that pool existed for, in descending order if no epoch number was provided)<br>
 [get_pool_updates](#get_pool_updates) Returns all pool updates for all pools or only updates for specific pool if specified<br>
@@ -1543,15 +1543,15 @@
     "block_time": 1670493734
   }
 ]
 ```
 
 ### Pool
 
-#### get_pools_list
+#### get_pool_list
 A list of all currently registered/retiring (not retired) pools<br>
 Parameters: none<br>
 Returns: The list of stake pool dictionaries<br>
 Example:<br>
 `pool_list = get_pool_list()`<br>
 Example response:
 ```json
```

### Comparing `koios-api-1.0.10/pyproject.toml` & `koios-api-1.0.10.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 [project]
 name = "koios-api"
-version = "1.0.10"
+version = "1.0.10.2"
 authors = [
   { name="APEX Stake Pool", email="cardanoapexpool@gmail.com" },
 ]
 description = "A python package for the Cardano Blockchain Koios API (https://api.koios.rest/)"
 keywords = [
     "koios",
     "cardano",
```

### Comparing `koios-api-1.0.10/src/koios_api/__config__.py` & `koios-api-1.0.10.2/src/koios_api/__config__.py`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10/src/koios_api/account.py` & `koios-api-1.0.10.2/src/koios_api/account.py`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10/src/koios_api/address.py` & `koios-api-1.0.10.2/src/koios_api/address.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,30 +36,42 @@
     Get the transaction hash list of input address array, optionally filtering after specified block height (inclusive)
     :param addr: Payment address(es) as string (for one address) or list (for multiple addresses)
     :param block_height: Return only the transactions after this block height. Optional.
     :returns: The list of transactions maps
     """
     url = API_BASE_URL + '/address_txs'
     headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
+    parameters = {}
     addresses = {}
     if isinstance(addr, list):
         addresses['_addresses'] = addr
     else:
         addresses['_addresses'] = [addr]
     if block_height > 0:
         addresses['_after_block_height'] = block_height
+    txs = []
+    offset = 0
     while True:
-        try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(addresses)).text)
-            break
-        except Exception as e:
-            print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
-            sleep(SLEEP_TIME)
+        if offset > 0:
+            parameters['offset'] = offset
+        while True:
+            try:
+                resp = json.loads(requests.post(url, headers=headers, params=parameters,
+                                                data=json.dumps(addresses)).text)
+                break
+            except Exception as e:
+                print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
+                sleep(SLEEP_TIME)
             print('retrying...')
-    return resp
+        txs += resp
+        if len(resp) < API_RESP_COUNT:
+            break
+        else:
+            offset += len(resp)
+    return txs
 
 
 def get_credential_utxos(cred: [str, list]) -> list:
     """
     https://api.koios.rest/#post-/credential_utxos
     Get a list of UTxO against input payment credential array including their balances
     :param cred: Payment credential in hex format as string (for one credential) or list (for multiple credentials)
```

### Comparing `koios-api-1.0.10/src/koios_api/asset.py` & `koios-api-1.0.10.2/src/koios_api/asset.py`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10/src/koios_api/block.py` & `koios-api-1.0.10.2/src/koios_api/block.py`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10/src/koios_api/epoch.py` & `koios-api-1.0.10.2/src/koios_api/epoch.py`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10/src/koios_api/network.py` & `koios-api-1.0.10.2/src/koios_api/network.py`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10/src/koios_api/pool.py` & `koios-api-1.0.10.2/src/koios_api/pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import requests
 import inspect
 from time import sleep
 from .__config__ import *
 
 
-def get_pools_list() -> list:
+def get_pool_list() -> list:
     """
     https://api.koios.rest/#get-/pool_list
     A list of all currently registered/retiring (not retired) pools
     :returns: The list of stake pool maps
     """
     url = API_BASE_URL + '/pool_list'
     headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
```

### Comparing `koios-api-1.0.10/src/koios_api/script.py` & `koios-api-1.0.10.2/src/koios_api/script.py`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10/src/koios_api/transactions.py` & `koios-api-1.0.10.2/src/koios_api/transactions.py`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10/src/koios_api.egg-info/PKG-INFO` & `koios-api-1.0.10.2/src/koios_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koios-api
-Version: 1.0.10
+Version: 1.0.10.2
 Summary: A python package for the Cardano Blockchain Koios API (https://api.koios.rest/)
 Author-email: APEX Stake Pool <cardanoapexpool@gmail.com>
 Project-URL: Homepage, https://github.com/cardano-apexpool/koios-api-python
 Project-URL: Bug Tracker, https://github.com/cardano-apexpool/koios-api-python/issues
 Keywords: koios,cardano,blockchain,REST,API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -111,15 +111,15 @@
 [get_policy_asset_addresses](#get_policy_asset_addresses) Get the list of addresses with quantity for each asset on the given policy<br>
 [get_policy_asset_info](#get_policy_asset_info) Get the information for all assets under the same policy<br>
 [get_policy_asset_list](#get_policy_asset_list) Get the list of asset under the given policy (including balances)<br>
 [get_asset_summary](#get_asset_summary) Get the summary of an asset (total transactions exclude minting/total wallets include only wallets with asset balance)<br>
 [get_asset_txs](#get_asset_txs) Get the list of all asset transaction hashes (the newest first)<br>
 
 [Pool](#Pool)<br>
-[get_pools_list](#get_pools_list) A list of all currently registered/retiring (not retired) pools<br>
+[get_pool_list](#get_pool_list) A list of all currently registered/retiring (not retired) pools<br>
 [get_pool_info](#get_pool_info) Current pool statuses and details for a specified list of pool ids<br>
 [get_pool_stake_snapshot](#get_pool_stake_snapshot) Returns Mark, Set and Go stake snapshots for the selected pool, useful for leaderlog calculation<br>
 [get_pool_delegators](#get_pool_delegators) Returns information about live delegators for a given pool<br>
 [get_pool_delegators_history](#get_pool_delegators_history) Returns information about active delegators (incl. history) for a given pool and epoch number (all epochs if not specified)<br>
 [get_pool_blocks](#get_pool_blocks) Returns information about blocks minted by a given pool for all epochs (or _epoch_no if provided)<br>
 [get_pool_history](#get_pool_history) Returns information about pool stake, block and reward history in a given epoch (or all epochs that pool existed for, in descending order if no epoch number was provided)<br>
 [get_pool_updates](#get_pool_updates) Returns all pool updates for all pools or only updates for specific pool if specified<br>
@@ -1558,15 +1558,15 @@
     "block_time": 1670493734
   }
 ]
 ```
 
 ### Pool
 
-#### get_pools_list
+#### get_pool_list
 A list of all currently registered/retiring (not retired) pools<br>
 Parameters: none<br>
 Returns: The list of stake pool dictionaries<br>
 Example:<br>
 `pool_list = get_pool_list()`<br>
 Example response:
 ```json
```

