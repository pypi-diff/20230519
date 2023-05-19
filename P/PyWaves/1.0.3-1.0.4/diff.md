# Comparing `tmp/PyWaves-1.0.3.tar.gz` & `tmp/PyWaves-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyWaves-1.0.3.tar", last modified: Mon Feb 27 16:19:58 2023, max compression
+gzip compressed data, was "PyWaves-1.0.4.tar", last modified: Fri May 19 06:31:11 2023, max compression
```

## Comparing `PyWaves-1.0.3.tar` & `PyWaves-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 marcjansen   (501) staff       (20)        0 2023-02-27 16:19:58.011489 PyWaves-1.0.3/
--rw-r--r--   0 marcjansen   (501) staff       (20)      298 2023-02-27 16:19:58.010683 PyWaves-1.0.3/PKG-INFO
-drwxr-xr-x   0 marcjansen   (501) staff       (20)        0 2023-02-27 16:19:57.981162 PyWaves-1.0.3/PyWaves.egg-info/
--rw-r--r--   0 marcjansen   (501) staff       (20)      298 2023-02-27 16:19:57.000000 PyWaves-1.0.3/PyWaves.egg-info/PKG-INFO
--rw-r--r--   0 marcjansen   (501) staff       (20)      630 2023-02-27 16:19:57.000000 PyWaves-1.0.3/PyWaves.egg-info/SOURCES.txt
--rw-r--r--   0 marcjansen   (501) staff       (20)        1 2023-02-27 16:19:57.000000 PyWaves-1.0.3/PyWaves.egg-info/dependency_links.txt
--rw-r--r--   0 marcjansen   (501) staff       (20)      100 2023-02-27 16:19:57.000000 PyWaves-1.0.3/PyWaves.egg-info/requires.txt
--rw-r--r--   0 marcjansen   (501) staff       (20)       48 2023-02-27 16:19:57.000000 PyWaves-1.0.3/PyWaves.egg-info/top_level.txt
-drwxr-xr-x   0 marcjansen   (501) staff       (20)        0 2023-02-27 16:19:57.998226 PyWaves-1.0.3/pywaves/
--rw-r--r--   0 marcjansen   (501) staff       (20)     6325 2022-10-11 07:41:58.000000 PyWaves-1.0.3/pywaves/ParallelPyWaves.py
--rw-r--r--   0 marcjansen   (501) staff       (20)     4768 2023-02-27 16:19:09.000000 PyWaves-1.0.3/pywaves/WXFeeCalculator.py
--rw-r--r--   0 marcjansen   (501) staff       (20)     5743 2022-12-29 16:50:51.000000 PyWaves-1.0.3/pywaves/__init__.py
--rw-r--r--   0 marcjansen   (501) staff       (20)    50687 2023-02-08 12:19:24.000000 PyWaves-1.0.3/pywaves/address.py
--rw-r--r--   0 marcjansen   (501) staff       (20)     6729 2023-02-03 10:00:27.000000 PyWaves-1.0.3/pywaves/asset.py
--rw-r--r--   0 marcjansen   (501) staff       (20)     1769 2022-07-19 20:05:17.000000 PyWaves-1.0.3/pywaves/contract.py
--rw-r--r--   0 marcjansen   (501) staff       (20)     7488 2019-12-02 05:09:27.000000 PyWaves-1.0.3/pywaves/crypto.py
--rw-r--r--   0 marcjansen   (501) staff       (20)     1366 2020-12-02 08:51:14.000000 PyWaves-1.0.3/pywaves/oracle.py
--rw-r--r--   0 marcjansen   (501) staff       (20)     1245 2020-02-21 10:40:35.000000 PyWaves-1.0.3/pywaves/order.py
-drwxr-xr-x   0 marcjansen   (501) staff       (20)        0 2023-02-27 16:19:57.971826 PyWaves-1.0.3/pywaves/protobuf/
-drwxr-xr-x   0 marcjansen   (501) staff       (20)        0 2023-02-27 16:19:58.009983 PyWaves-1.0.3/pywaves/protobuf/waves/
--rw-r--r--   0 marcjansen   (501) staff       (20)     2646 2023-02-08 12:19:24.000000 PyWaves-1.0.3/pywaves/protobuf/waves/amount_pb2.py
--rw-r--r--   0 marcjansen   (501) staff       (20)    14336 2023-02-08 12:19:24.000000 PyWaves-1.0.3/pywaves/protobuf/waves/block_pb2.py
--rw-r--r--   0 marcjansen   (501) staff       (20)    39769 2023-02-08 12:19:24.000000 PyWaves-1.0.3/pywaves/protobuf/waves/invoke_script_result_pb2.py
--rw-r--r--   0 marcjansen   (501) staff       (20)    12672 2023-02-08 12:19:24.000000 PyWaves-1.0.3/pywaves/protobuf/waves/order_pb2.py
--rw-r--r--   0 marcjansen   (501) staff       (20)     3357 2023-02-08 12:19:24.000000 PyWaves-1.0.3/pywaves/protobuf/waves/recipient_pb2.py
--rw-r--r--   0 marcjansen   (501) staff       (20)    65284 2023-02-08 12:19:24.000000 PyWaves-1.0.3/pywaves/protobuf/waves/transaction_pb2.py
--rw-r--r--   0 marcjansen   (501) staff       (20)    11720 2023-02-08 12:19:24.000000 PyWaves-1.0.3/pywaves/txGenerator.py
--rw-r--r--   0 marcjansen   (501) staff       (20)    22735 2023-02-08 12:19:24.000000 PyWaves-1.0.3/pywaves/txSigner.py
--rw-r--r--   0 marcjansen   (501) staff       (20)       38 2023-02-27 16:19:58.011543 PyWaves-1.0.3/setup.cfg
--rw-r--r--   0 marcjansen   (501) staff       (20)      635 2023-02-27 16:19:44.000000 PyWaves-1.0.3/setup.py
+drwxr-xr-x   0 marcjansen   (501) staff       (20)        0 2023-05-19 06:31:11.799388 PyWaves-1.0.4/
+-rw-r--r--   0 marcjansen   (501) staff       (20)      298 2023-05-19 06:31:11.798009 PyWaves-1.0.4/PKG-INFO
+drwxr-xr-x   0 marcjansen   (501) staff       (20)        0 2023-05-19 06:31:11.529548 PyWaves-1.0.4/PyWaves.egg-info/
+-rw-r--r--   0 marcjansen   (501) staff       (20)      298 2023-05-19 06:31:11.000000 PyWaves-1.0.4/PyWaves.egg-info/PKG-INFO
+-rw-r--r--   0 marcjansen   (501) staff       (20)      630 2023-05-19 06:31:11.000000 PyWaves-1.0.4/PyWaves.egg-info/SOURCES.txt
+-rw-r--r--   0 marcjansen   (501) staff       (20)        1 2023-05-19 06:31:11.000000 PyWaves-1.0.4/PyWaves.egg-info/dependency_links.txt
+-rw-r--r--   0 marcjansen   (501) staff       (20)      100 2023-05-19 06:31:11.000000 PyWaves-1.0.4/PyWaves.egg-info/requires.txt
+-rw-r--r--   0 marcjansen   (501) staff       (20)       48 2023-05-19 06:31:11.000000 PyWaves-1.0.4/PyWaves.egg-info/top_level.txt
+drwxr-xr-x   0 marcjansen   (501) staff       (20)        0 2023-05-19 06:31:11.727221 PyWaves-1.0.4/pywaves/
+-rw-r--r--   0 marcjansen   (501) staff       (20)     6325 2022-10-11 07:41:58.000000 PyWaves-1.0.4/pywaves/ParallelPyWaves.py
+-rw-r--r--   0 marcjansen   (501) staff       (20)     4700 2023-05-19 06:29:04.000000 PyWaves-1.0.4/pywaves/WXFeeCalculator.py
+-rw-r--r--   0 marcjansen   (501) staff       (20)     5743 2022-12-29 16:50:51.000000 PyWaves-1.0.4/pywaves/__init__.py
+-rw-r--r--   0 marcjansen   (501) staff       (20)    50687 2023-02-08 12:19:24.000000 PyWaves-1.0.4/pywaves/address.py
+-rw-r--r--   0 marcjansen   (501) staff       (20)     6729 2023-02-03 10:00:27.000000 PyWaves-1.0.4/pywaves/asset.py
+-rw-r--r--   0 marcjansen   (501) staff       (20)     1769 2022-07-19 20:05:17.000000 PyWaves-1.0.4/pywaves/contract.py
+-rw-r--r--   0 marcjansen   (501) staff       (20)     7488 2019-12-02 05:09:27.000000 PyWaves-1.0.4/pywaves/crypto.py
+-rw-r--r--   0 marcjansen   (501) staff       (20)     1366 2020-12-02 08:51:14.000000 PyWaves-1.0.4/pywaves/oracle.py
+-rw-r--r--   0 marcjansen   (501) staff       (20)     1245 2020-02-21 10:40:35.000000 PyWaves-1.0.4/pywaves/order.py
+drwxr-xr-x   0 marcjansen   (501) staff       (20)        0 2023-05-19 06:31:11.513749 PyWaves-1.0.4/pywaves/protobuf/
+drwxr-xr-x   0 marcjansen   (501) staff       (20)        0 2023-05-19 06:31:11.796208 PyWaves-1.0.4/pywaves/protobuf/waves/
+-rw-r--r--   0 marcjansen   (501) staff       (20)     2646 2023-02-08 12:19:24.000000 PyWaves-1.0.4/pywaves/protobuf/waves/amount_pb2.py
+-rw-r--r--   0 marcjansen   (501) staff       (20)    14336 2023-02-08 12:19:24.000000 PyWaves-1.0.4/pywaves/protobuf/waves/block_pb2.py
+-rw-r--r--   0 marcjansen   (501) staff       (20)    39769 2023-02-08 12:19:24.000000 PyWaves-1.0.4/pywaves/protobuf/waves/invoke_script_result_pb2.py
+-rw-r--r--   0 marcjansen   (501) staff       (20)    12672 2023-02-08 12:19:24.000000 PyWaves-1.0.4/pywaves/protobuf/waves/order_pb2.py
+-rw-r--r--   0 marcjansen   (501) staff       (20)     3357 2023-02-08 12:19:24.000000 PyWaves-1.0.4/pywaves/protobuf/waves/recipient_pb2.py
+-rw-r--r--   0 marcjansen   (501) staff       (20)    65284 2023-02-08 12:19:24.000000 PyWaves-1.0.4/pywaves/protobuf/waves/transaction_pb2.py
+-rw-r--r--   0 marcjansen   (501) staff       (20)    11720 2023-02-08 12:19:24.000000 PyWaves-1.0.4/pywaves/txGenerator.py
+-rw-r--r--   0 marcjansen   (501) staff       (20)    22876 2023-05-19 06:29:04.000000 PyWaves-1.0.4/pywaves/txSigner.py
+-rw-r--r--   0 marcjansen   (501) staff       (20)       38 2023-05-19 06:31:11.800741 PyWaves-1.0.4/setup.cfg
+-rw-r--r--   0 marcjansen   (501) staff       (20)      635 2023-05-19 06:30:40.000000 PyWaves-1.0.4/setup.py
```

### Comparing `PyWaves-1.0.3/PyWaves.egg-info/SOURCES.txt` & `PyWaves-1.0.4/PyWaves.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyWaves-1.0.3/pywaves/ParallelPyWaves.py` & `PyWaves-1.0.4/pywaves/ParallelPyWaves.py`

 * *Files identical despite different names*

### Comparing `PyWaves-1.0.3/pywaves/WXFeeCalculator.py` & `PyWaves-1.0.4/pywaves/WXFeeCalculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,14 @@
         amountAssetDecimals = self._getAssetDecimals(amountAssetId)
         price = price / math.pow(10, priceAssetDecimals)
         amount = amountToBuy / math.pow(10, amountAssetDecimals)
         calculatedFee = amount * price * minFee / 100
         calculatedFee = int(calculatedFee * math.pow(10, priceAssetDecimals))
         minFee = self._getMinFee(priceAssetId)
 
-        minFee = minFee / math.pow(10, 8 - priceAssetDecimals) + 1
-
         return int(max(calculatedFee, minFee))
 
     def calculatePercentDiscountedBuyingFee(self, priceAssetId, price, amountToBuy):
         discount = self.settings['orderFee']['composite']['discount']['value']
         discountAssetId = self.settings['orderFee']['composite']['discount']['assetId']
         rates = self.settings['rates']
         discountAssetRate = self._correctRate(rates[discountAssetId], self.discountAssetDecimals)
```

### Comparing `PyWaves-1.0.3/pywaves/__init__.py` & `PyWaves-1.0.4/pywaves/__init__.py`

 * *Files identical despite different names*

### Comparing `PyWaves-1.0.3/pywaves/address.py` & `PyWaves-1.0.4/pywaves/address.py`

 * *Files identical despite different names*

### Comparing `PyWaves-1.0.3/pywaves/asset.py` & `PyWaves-1.0.4/pywaves/asset.py`

 * *Files identical despite different names*

### Comparing `PyWaves-1.0.3/pywaves/contract.py` & `PyWaves-1.0.4/pywaves/contract.py`

 * *Files identical despite different names*

### Comparing `PyWaves-1.0.3/pywaves/crypto.py` & `PyWaves-1.0.4/pywaves/crypto.py`

 * *Files identical despite different names*

### Comparing `PyWaves-1.0.3/pywaves/oracle.py` & `PyWaves-1.0.4/pywaves/oracle.py`

 * *Files identical despite different names*

### Comparing `PyWaves-1.0.3/pywaves/order.py` & `PyWaves-1.0.4/pywaves/order.py`

 * *Files identical despite different names*

### Comparing `PyWaves-1.0.3/pywaves/protobuf/waves/amount_pb2.py` & `PyWaves-1.0.4/pywaves/protobuf/waves/amount_pb2.py`

 * *Files identical despite different names*

### Comparing `PyWaves-1.0.3/pywaves/protobuf/waves/block_pb2.py` & `PyWaves-1.0.4/pywaves/protobuf/waves/block_pb2.py`

 * *Files identical despite different names*

### Comparing `PyWaves-1.0.3/pywaves/protobuf/waves/invoke_script_result_pb2.py` & `PyWaves-1.0.4/pywaves/protobuf/waves/invoke_script_result_pb2.py`

 * *Files identical despite different names*

### Comparing `PyWaves-1.0.3/pywaves/protobuf/waves/order_pb2.py` & `PyWaves-1.0.4/pywaves/protobuf/waves/order_pb2.py`

 * *Files identical despite different names*

### Comparing `PyWaves-1.0.3/pywaves/protobuf/waves/recipient_pb2.py` & `PyWaves-1.0.4/pywaves/protobuf/waves/recipient_pb2.py`

 * *Files identical despite different names*

### Comparing `PyWaves-1.0.3/pywaves/protobuf/waves/transaction_pb2.py` & `PyWaves-1.0.4/pywaves/protobuf/waves/transaction_pb2.py`

 * *Files identical despite different names*

### Comparing `PyWaves-1.0.3/pywaves/txGenerator.py` & `PyWaves-1.0.4/pywaves/txGenerator.py`

 * *Files identical despite different names*

### Comparing `PyWaves-1.0.3/pywaves/txSigner.py` & `PyWaves-1.0.4/pywaves/txSigner.py`

 * *Files 1% similar despite different names*

```diff
@@ -441,43 +441,44 @@
         transaction.update_asset_info.CopyFrom(updateInfo)
 
         proof = crypto.sign(privateKey, transaction.SerializeToString())
         tx['proofs'].append(proof)
 
     def signType16Tx(self, tx, privateKey):
         parameterBytes = b''
-        for param in tx['call']['args']:
-            if param['type'] == 'integer':
-                parameterBytes += b'\0' + struct.pack(">q", param['value'])
-            elif param['type'] == 'binary':
-                parameterBytes += b'\1' + struct.pack(">L", len(param['value'])) + crypto.str2bytes(param['value'])
-            elif param['type'] == 'string':
-                parameterBytes += b'\2' + struct.pack(">I", len(crypto.str2bytes(param['value']))) + crypto.str2bytes(
-                    param['value'])
-            elif param['type'] == 'boolean':
-                if param['value'] == True:
-                    parameterBytes += b'\6'
-                else:
-                    parameterBytes += b'\7'
-            elif param['type'] == 'list':
-                parameterBytes += b'\x0b'
-                parameterBytes += struct.pack(">I", len(param['value']))
-                for nestedParam in param['value']:
-                    if nestedParam['type'] == 'integer':
-                        parameterBytes += b'\0' + struct.pack(">Q", nestedParam['value'])
-                    elif nestedParam['type'] == 'binary':
-                        parameterBytes += b'\1' + struct.pack(">I", len(nestedParam['value'])) + crypto.str2bytes(nestedParam['value'])
-                    elif nestedParam['type'] == 'string':
-                        parameterBytes += b'\2' + struct.pack(">I", len(crypto.str2bytes(
-                            nestedParam['value']))) + crypto.str2bytes(nestedParam['value'])
-                    elif nestedParam['type'] == 'boolean':
-                        if nestedParam['value'] == True:
-                            parameterBytes += b'\6'
-                        else:
-                            parameterBytes += b'\7'
+        if 'call' in tx:
+            for param in tx['call']['args']:
+                if param['type'] == 'integer':
+                    parameterBytes += b'\0' + struct.pack(">q", param['value'])
+                elif param['type'] == 'binary':
+                    parameterBytes += b'\1' + struct.pack(">L", len(param['value'])) + crypto.str2bytes(param['value'])
+                elif param['type'] == 'string':
+                    parameterBytes += b'\2' + struct.pack(">I", len(crypto.str2bytes(param['value']))) + crypto.str2bytes(
+                        param['value'])
+                elif param['type'] == 'boolean':
+                    if param['value'] == True:
+                        parameterBytes += b'\6'
+                    else:
+                        parameterBytes += b'\7'
+                elif param['type'] == 'list':
+                    parameterBytes += b'\x0b'
+                    parameterBytes += struct.pack(">I", len(param['value']))
+                    for nestedParam in param['value']:
+                        if nestedParam['type'] == 'integer':
+                            parameterBytes += b'\0' + struct.pack(">Q", nestedParam['value'])
+                        elif nestedParam['type'] == 'binary':
+                            parameterBytes += b'\1' + struct.pack(">I", len(nestedParam['value'])) + crypto.str2bytes(nestedParam['value'])
+                        elif nestedParam['type'] == 'string':
+                            parameterBytes += b'\2' + struct.pack(">I", len(crypto.str2bytes(
+                                nestedParam['value']))) + crypto.str2bytes(nestedParam['value'])
+                        elif nestedParam['type'] == 'boolean':
+                            if nestedParam['value'] == True:
+                                parameterBytes += b'\6'
+                            else:
+                                parameterBytes += b'\7'
         invoke = transaction_pb2.InvokeScriptTransactionData()
         for payment in tx['payment']:
             amount = amount_pb2.Amount()
             amount.amount = payment['amount']
             if not ('assetId' not in payment or payment['assetId'] == 'null' or payment['assetId'] == None or payment['assetId'] == ''):
                 amount.asset_id = base58.b58decode(payment['assetId'])
             invoke.payments.append(amount)
```

### Comparing `PyWaves-1.0.3/setup.py` & `PyWaves-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='PyWaves',
-      version='1.0.3',
+      version='1.0.4',
       description='Object-oriented library for the Waves blockchain platform',
       url='http://github.com/pywaves/pywaves',
       author='PyWaves Developers',
       author_email='dev@pywaves.org',
       license='MIT',
       packages=['pywaves', 'pywaves/protobuf', 'pywaves/protobuf/waves'],
       keywords = ['waves', 'blockchain', 'analytics'],
```

