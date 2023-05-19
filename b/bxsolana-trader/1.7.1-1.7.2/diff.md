# Comparing `tmp/bxsolana-trader-1.7.1.tar.gz` & `tmp/bxsolana-trader-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bxsolana-trader-1.7.1.tar", last modified: Mon May 15 18:31:01 2023, max compression
+gzip compressed data, was "bxsolana-trader-1.7.2.tar", last modified: Fri May 19 16:16:07 2023, max compression
```

## Comparing `bxsolana-trader-1.7.1.tar` & `bxsolana-trader-1.7.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 18:31:01.546609 bxsolana-trader-1.7.1/
--rw-r--r--   0 aspin      (501) staff       (20)     1071 2022-09-13 19:43:40.000000 bxsolana-trader-1.7.1/LICENSE
--rw-r--r--   0 aspin      (501) staff       (20)     4348 2023-05-15 18:31:01.546692 bxsolana-trader-1.7.1/PKG-INFO
--rw-r--r--   0 aspin      (501) staff       (20)     2867 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.1/README.md
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 18:31:01.539401 bxsolana-trader-1.7.1/bxsolana/
--rw-r--r--   0 aspin      (501) staff       (20)      280 2023-01-10 20:47:33.000000 bxsolana-trader-1.7.1/bxsolana/__init__.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 18:31:01.541402 bxsolana-trader-1.7.1/bxsolana/examples/
--rw-r--r--   0 aspin      (501) staff       (20)      670 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.1/bxsolana/examples/__init__.py
--rw-r--r--   0 aspin      (501) staff       (20)      617 2023-02-21 21:35:54.000000 bxsolana-trader-1.7.1/bxsolana/examples/constants.py
--rw-r--r--   0 aspin      (501) staff       (20)     2727 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.1/bxsolana/examples/order_lifecycle.py
--rw-r--r--   0 aspin      (501) staff       (20)     7864 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.1/bxsolana/examples/order_utils.py
--rw-r--r--   0 aspin      (501) staff       (20)    19105 2023-05-15 18:13:59.000000 bxsolana-trader-1.7.1/bxsolana/examples/request_utils.py
--rw-r--r--   0 aspin      (501) staff       (20)     4708 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.1/bxsolana/examples/stream_utils.py
--rw-r--r--   0 aspin      (501) staff       (20)     5851 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.1/bxsolana/examples/transaction_request_utils.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 18:31:01.543056 bxsolana-trader-1.7.1/bxsolana/provider/
--rw-r--r--   0 aspin      (501) staff       (20)      582 2022-10-10 22:32:15.000000 bxsolana-trader-1.7.1/bxsolana/provider/__init__.py
--rw-r--r--   0 aspin      (501) staff       (20)    11768 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.1/bxsolana/provider/base.py
--rw-r--r--   0 aspin      (501) staff       (20)      970 2023-02-20 23:04:33.000000 bxsolana-trader-1.7.1/bxsolana/provider/constants.py
--rw-r--r--   0 aspin      (501) staff       (20)     2662 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.1/bxsolana/provider/grpc.py
--rw-r--r--   0 aspin      (501) staff       (20)    30225 2023-05-15 18:29:17.000000 bxsolana-trader-1.7.1/bxsolana/provider/http.py
--rw-r--r--   0 aspin      (501) staff       (20)      947 2023-03-06 23:02:29.000000 bxsolana-trader-1.7.1/bxsolana/provider/http_error.py
--rw-r--r--   0 aspin      (501) staff       (20)     4201 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.1/bxsolana/provider/ws.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 18:31:01.543708 bxsolana-trader-1.7.1/bxsolana/transaction/
--rw-r--r--   0 aspin      (501) staff       (20)      593 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.1/bxsolana/transaction/__init__.py
--rw-r--r--   0 aspin      (501) staff       (20)     2361 2023-03-14 21:50:18.000000 bxsolana-trader-1.7.1/bxsolana/transaction/memo.py
--rw-r--r--   0 aspin      (501) staff       (20)     2402 2023-03-14 21:50:18.000000 bxsolana-trader-1.7.1/bxsolana/transaction/signing.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 18:31:01.544370 bxsolana-trader-1.7.1/bxsolana_trader.egg-info/
--rw-r--r--   0 aspin      (501) staff       (20)     4348 2023-05-15 18:31:01.000000 bxsolana-trader-1.7.1/bxsolana_trader.egg-info/PKG-INFO
--rw-r--r--   0 aspin      (501) staff       (20)     1138 2023-05-15 18:31:01.000000 bxsolana-trader-1.7.1/bxsolana_trader.egg-info/SOURCES.txt
--rw-r--r--   0 aspin      (501) staff       (20)        1 2023-05-15 18:31:01.000000 bxsolana-trader-1.7.1/bxsolana_trader.egg-info/dependency_links.txt
--rw-r--r--   0 aspin      (501) staff       (20)      145 2023-05-15 18:31:01.000000 bxsolana-trader-1.7.1/bxsolana_trader.egg-info/requires.txt
--rw-r--r--   0 aspin      (501) staff       (20)       14 2023-05-15 18:31:01.000000 bxsolana-trader-1.7.1/bxsolana_trader.egg-info/top_level.txt
--rw-r--r--   0 aspin      (501) staff       (20)      217 2022-09-07 21:30:01.000000 bxsolana-trader-1.7.1/pyproject.toml
--rw-r--r--   0 aspin      (501) staff       (20)      677 2023-05-15 18:31:01.546984 bxsolana-trader-1.7.1/setup.cfg
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 18:31:01.544477 bxsolana-trader-1.7.1/test/
--rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.1/test/__init__.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 18:31:01.545987 bxsolana-trader-1.7.1/test/integration/
--rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.1/test/integration/__init__.py
--rw-r--r--   0 aspin      (501) staff       (20)     4020 2023-02-20 23:04:33.000000 bxsolana-trader-1.7.1/test/integration/private.py
--rw-r--r--   0 aspin      (501) staff       (20)     2192 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.1/test/integration/public.py
--rw-r--r--   0 aspin      (501) staff       (20)      852 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.1/test/integration/stream.py
--rw-r--r--   0 aspin      (501) staff       (20)      701 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.1/test/integration/test_grpc.py
--rw-r--r--   0 aspin      (501) staff       (20)      544 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.1/test/integration/test_http.py
--rw-r--r--   0 aspin      (501) staff       (20)      664 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.1/test/integration/test_ws.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 18:31:01.546178 bxsolana-trader-1.7.1/test/unit/
--rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.1/test/unit/__init__.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-15 18:31:01.546489 bxsolana-trader-1.7.1/test/unit/transaction/
--rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.1/test/unit/transaction/__init__.py
--rw-r--r--   0 aspin      (501) staff       (20)     1386 2023-03-14 21:50:18.000000 bxsolana-trader-1.7.1/test/unit/transaction/test_memo.py
--rw-r--r--   0 aspin      (501) staff       (20)     4629 2023-03-14 21:50:18.000000 bxsolana-trader-1.7.1/test/unit/transaction/test_signing.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-19 16:16:07.951733 bxsolana-trader-1.7.2/
+-rw-r--r--   0 aspin      (501) staff       (20)     1071 2022-09-13 19:43:40.000000 bxsolana-trader-1.7.2/LICENSE
+-rw-r--r--   0 aspin      (501) staff       (20)     4348 2023-05-19 16:16:07.951806 bxsolana-trader-1.7.2/PKG-INFO
+-rw-r--r--   0 aspin      (501) staff       (20)     2867 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.2/README.md
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-19 16:16:07.931781 bxsolana-trader-1.7.2/bxsolana/
+-rw-r--r--   0 aspin      (501) staff       (20)      280 2023-01-10 20:47:33.000000 bxsolana-trader-1.7.2/bxsolana/__init__.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-19 16:16:07.934651 bxsolana-trader-1.7.2/bxsolana/examples/
+-rw-r--r--   0 aspin      (501) staff       (20)      670 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.2/bxsolana/examples/__init__.py
+-rw-r--r--   0 aspin      (501) staff       (20)      617 2023-02-21 21:35:54.000000 bxsolana-trader-1.7.2/bxsolana/examples/constants.py
+-rw-r--r--   0 aspin      (501) staff       (20)     2727 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.2/bxsolana/examples/order_lifecycle.py
+-rw-r--r--   0 aspin      (501) staff       (20)     7864 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.2/bxsolana/examples/order_utils.py
+-rw-r--r--   0 aspin      (501) staff       (20)    19397 2023-05-19 16:15:42.000000 bxsolana-trader-1.7.2/bxsolana/examples/request_utils.py
+-rw-r--r--   0 aspin      (501) staff       (20)     5177 2023-05-19 16:15:42.000000 bxsolana-trader-1.7.2/bxsolana/examples/stream_utils.py
+-rw-r--r--   0 aspin      (501) staff       (20)     5851 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.2/bxsolana/examples/transaction_request_utils.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-19 16:16:07.942780 bxsolana-trader-1.7.2/bxsolana/provider/
+-rw-r--r--   0 aspin      (501) staff       (20)      582 2022-10-10 22:32:15.000000 bxsolana-trader-1.7.2/bxsolana/provider/__init__.py
+-rw-r--r--   0 aspin      (501) staff       (20)    11768 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.2/bxsolana/provider/base.py
+-rw-r--r--   0 aspin      (501) staff       (20)      970 2023-02-20 23:04:33.000000 bxsolana-trader-1.7.2/bxsolana/provider/constants.py
+-rw-r--r--   0 aspin      (501) staff       (20)     2662 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.2/bxsolana/provider/grpc.py
+-rw-r--r--   0 aspin      (501) staff       (20)    30859 2023-05-19 16:15:42.000000 bxsolana-trader-1.7.2/bxsolana/provider/http.py
+-rw-r--r--   0 aspin      (501) staff       (20)      947 2023-03-06 23:02:29.000000 bxsolana-trader-1.7.2/bxsolana/provider/http_error.py
+-rw-r--r--   0 aspin      (501) staff       (20)     4201 2023-05-15 16:27:33.000000 bxsolana-trader-1.7.2/bxsolana/provider/ws.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-19 16:16:07.944325 bxsolana-trader-1.7.2/bxsolana/transaction/
+-rw-r--r--   0 aspin      (501) staff       (20)      593 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.2/bxsolana/transaction/__init__.py
+-rw-r--r--   0 aspin      (501) staff       (20)     2361 2023-03-14 21:50:18.000000 bxsolana-trader-1.7.2/bxsolana/transaction/memo.py
+-rw-r--r--   0 aspin      (501) staff       (20)     2402 2023-03-14 21:50:18.000000 bxsolana-trader-1.7.2/bxsolana/transaction/signing.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-19 16:16:07.949278 bxsolana-trader-1.7.2/bxsolana_trader.egg-info/
+-rw-r--r--   0 aspin      (501) staff       (20)     4348 2023-05-19 16:16:07.000000 bxsolana-trader-1.7.2/bxsolana_trader.egg-info/PKG-INFO
+-rw-r--r--   0 aspin      (501) staff       (20)     1138 2023-05-19 16:16:07.000000 bxsolana-trader-1.7.2/bxsolana_trader.egg-info/SOURCES.txt
+-rw-r--r--   0 aspin      (501) staff       (20)        1 2023-05-19 16:16:07.000000 bxsolana-trader-1.7.2/bxsolana_trader.egg-info/dependency_links.txt
+-rw-r--r--   0 aspin      (501) staff       (20)      145 2023-05-19 16:16:07.000000 bxsolana-trader-1.7.2/bxsolana_trader.egg-info/requires.txt
+-rw-r--r--   0 aspin      (501) staff       (20)       14 2023-05-19 16:16:07.000000 bxsolana-trader-1.7.2/bxsolana_trader.egg-info/top_level.txt
+-rw-r--r--   0 aspin      (501) staff       (20)      217 2022-09-07 21:30:01.000000 bxsolana-trader-1.7.2/pyproject.toml
+-rw-r--r--   0 aspin      (501) staff       (20)      677 2023-05-19 16:16:07.952345 bxsolana-trader-1.7.2/setup.cfg
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-19 16:16:07.949410 bxsolana-trader-1.7.2/test/
+-rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.2/test/__init__.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-19 16:16:07.951027 bxsolana-trader-1.7.2/test/integration/
+-rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.2/test/integration/__init__.py
+-rw-r--r--   0 aspin      (501) staff       (20)     4020 2023-02-20 23:04:33.000000 bxsolana-trader-1.7.2/test/integration/private.py
+-rw-r--r--   0 aspin      (501) staff       (20)     2192 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.2/test/integration/public.py
+-rw-r--r--   0 aspin      (501) staff       (20)      852 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.2/test/integration/stream.py
+-rw-r--r--   0 aspin      (501) staff       (20)      701 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.2/test/integration/test_grpc.py
+-rw-r--r--   0 aspin      (501) staff       (20)      544 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.2/test/integration/test_http.py
+-rw-r--r--   0 aspin      (501) staff       (20)      664 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.2/test/integration/test_ws.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-19 16:16:07.951197 bxsolana-trader-1.7.2/test/unit/
+-rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.2/test/unit/__init__.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-05-19 16:16:07.951594 bxsolana-trader-1.7.2/test/unit/transaction/
+-rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.7.2/test/unit/transaction/__init__.py
+-rw-r--r--   0 aspin      (501) staff       (20)     1386 2023-03-14 21:50:18.000000 bxsolana-trader-1.7.2/test/unit/transaction/test_memo.py
+-rw-r--r--   0 aspin      (501) staff       (20)     4629 2023-03-14 21:50:18.000000 bxsolana-trader-1.7.2/test/unit/transaction/test_signing.py
```

### Comparing `bxsolana-trader-1.7.1/LICENSE` & `bxsolana-trader-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/PKG-INFO` & `bxsolana-trader-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bxsolana-trader
-Version: 1.7.1
+Version: 1.7.2
 Summary: Python SDK for bloXroute's Solana Trader API
 Home-page: https://github.com/bloXroute-Labs/solana-trader-client-python
 Author: bloXroute Labs
 Author-email: support@bloxroute.com
 Keywords: serum,solana,blockchain,trader,grpc,stream
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `bxsolana-trader-1.7.1/README.md` & `bxsolana-trader-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/bxsolana/examples/__init__.py` & `bxsolana-trader-1.7.2/bxsolana/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/bxsolana/examples/constants.py` & `bxsolana-trader-1.7.2/bxsolana/examples/constants.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/bxsolana/examples/order_lifecycle.py` & `bxsolana-trader-1.7.2/bxsolana/examples/order_lifecycle.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/bxsolana/examples/order_utils.py` & `bxsolana-trader-1.7.2/bxsolana/examples/order_utils.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/bxsolana/examples/request_utils.py` & `bxsolana-trader-1.7.2/bxsolana/examples/request_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,14 +385,25 @@
                     contract=PerpContract.SOL_PERP,
                     project=proto.Project.P_DRIFT,
                 )
             )
         ).to_json()
     )
 
+    print("get Drift market depth")
+    print(
+        (
+            await api.get_drift_market_depth(
+                get_drift_market_depth_request=proto.GetDriftMarketDepthRequest(
+                    contract="SOL_PERP", limit=3
+                )
+            )
+        ).to_json()
+    )
+
     print("post perp order")
     print(
         (
             await api.post_perp_order(
                 post_perp_order_request=proto.PostPerpOrderRequest(
                     project=proto.Project.P_DRIFT,
                     owner_address=public_key,
```

### Comparing `bxsolana-trader-1.7.1/bxsolana/examples/stream_utils.py` & `bxsolana-trader-1.7.2/bxsolana/examples/stream_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,7 +133,20 @@
             )
         ):
             print(response.to_json())
             item_count += 1
             if item_count == 1:
                 item_count = 0
                 break
+
+    if run_slow:
+        print("streaming Drift market depth updates...")
+        async for response in api.get_drift_market_depths_stream(
+            get_drift_market_depths_stream_request=proto.GetDriftMarketDepthsStreamRequest(
+                contracts=["SOL_PERP", "ETH_PERP"], limit=3
+            )
+        ):
+            print(response.to_json())
+            item_count += 1
+            if item_count == 2:
+                item_count = 0
+                break
```

### Comparing `bxsolana-trader-1.7.1/bxsolana/examples/transaction_request_utils.py` & `bxsolana-trader-1.7.2/bxsolana/examples/transaction_request_utils.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/bxsolana/provider/__init__.py` & `bxsolana-trader-1.7.2/bxsolana/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/bxsolana/provider/base.py` & `bxsolana-trader-1.7.2/bxsolana/provider/base.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/bxsolana/provider/constants.py` & `bxsolana-trader-1.7.2/bxsolana/provider/constants.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/bxsolana/provider/grpc.py` & `bxsolana-trader-1.7.2/bxsolana/provider/grpc.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/bxsolana/provider/http.py` & `bxsolana-trader-1.7.2/bxsolana/provider/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
     # noinspection PyProtectedMember
     from betterproto import T
 
 
 class HttpProvider(Provider):
     _endpoint: str
+    _endpointV2: str
     _session: aiohttp.ClientSession
     _private_key: Optional[kp.Keypair]
 
     # noinspection PyMissingConstructor
     def __init__(
         self,
         endpoint: str = constants.MAINNET_API_HTTP,
@@ -338,14 +339,28 @@
     ) -> proto.GetPerpOrderbookResponse:
         async with self._session.get(
             f"{self._endpoint}/market/perp/orderbook/{get_perp_orderbook_request.contract}?"
             f"limit={get_perp_orderbook_request.limit}&project={get_perp_orderbook_request.project.name}"
         ) as res:
             return await map_response(res, proto.GetPerpOrderbookResponse())
 
+    async def get_drift_market_depth(
+        self,
+        get_drift_market_depth_request: proto.GetDriftMarketDepthRequest,
+        *,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> proto.GetDriftMarketDepthResponse:
+        async with self._session.get(
+            f"{self._endpointV2}/drift/market-depth/{get_drift_market_depth_request.contract}?"
+            f"limit={get_drift_market_depth_request.limit}"
+        ) as res:
+            return await map_response(res, proto.GetDriftMarketDepthResponse())
+
     async def post_settle_pnl(
         self,
         post_settle_pnl_request: proto.PostSettlePnlRequest,
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
```

### Comparing `bxsolana-trader-1.7.1/bxsolana/provider/http_error.py` & `bxsolana-trader-1.7.2/bxsolana/provider/http_error.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/bxsolana/provider/ws.py` & `bxsolana-trader-1.7.2/bxsolana/provider/ws.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/bxsolana/transaction/__init__.py` & `bxsolana-trader-1.7.2/bxsolana/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/bxsolana/transaction/memo.py` & `bxsolana-trader-1.7.2/bxsolana/transaction/memo.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/bxsolana/transaction/signing.py` & `bxsolana-trader-1.7.2/bxsolana/transaction/signing.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/bxsolana_trader.egg-info/PKG-INFO` & `bxsolana-trader-1.7.2/bxsolana_trader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bxsolana-trader
-Version: 1.7.1
+Version: 1.7.2
 Summary: Python SDK for bloXroute's Solana Trader API
 Home-page: https://github.com/bloXroute-Labs/solana-trader-client-python
 Author: bloXroute Labs
 Author-email: support@bloxroute.com
 Keywords: serum,solana,blockchain,trader,grpc,stream
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `bxsolana-trader-1.7.1/bxsolana_trader.egg-info/SOURCES.txt` & `bxsolana-trader-1.7.2/bxsolana_trader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/setup.cfg` & `bxsolana-trader-1.7.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bxsolana-trader
-version = 1.7.1
+version = 1.7.2
 description = Python SDK for bloXroute's Solana Trader API
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 author = bloXroute Labs
 author_email = support@bloxroute.com
 url = https://github.com/bloXroute-Labs/solana-trader-client-python
 keywords = serum, solana, blockchain, trader, grpc, stream
```

### Comparing `bxsolana-trader-1.7.1/test/integration/private.py` & `bxsolana-trader-1.7.2/test/integration/private.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/test/integration/public.py` & `bxsolana-trader-1.7.2/test/integration/public.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/test/integration/stream.py` & `bxsolana-trader-1.7.2/test/integration/stream.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/test/integration/test_grpc.py` & `bxsolana-trader-1.7.2/test/integration/test_grpc.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/test/integration/test_http.py` & `bxsolana-trader-1.7.2/test/integration/test_http.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/test/integration/test_ws.py` & `bxsolana-trader-1.7.2/test/integration/test_ws.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/test/unit/transaction/test_memo.py` & `bxsolana-trader-1.7.2/test/unit/transaction/test_memo.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.7.1/test/unit/transaction/test_signing.py` & `bxsolana-trader-1.7.2/test/unit/transaction/test_signing.py`

 * *Files identical despite different names*

